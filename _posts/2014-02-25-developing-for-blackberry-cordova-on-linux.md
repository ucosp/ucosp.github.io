---
id: 2946
title: Developing for Blackberry Cordova on Linux
date: 2014-02-25T15:17:24+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2946
permalink: /winter-2014/2014/02/developing-for-blackberry-cordova-on-linux/
categories:
  - Winter 2014
---
James Wood from Waterloo is working on Blackberry Cordova plugins on Linux and provides this reference for future developers who are trying to do the same.

### History

As of this writing, Linux is not supported by Blackberry for development, which means if you are reading this, that you have chosen to walk the difficult path. The good news is that you won&#8217;t be alone, and hopefully this guide will help get you started. The bad news is that a similar guide was written about four months before this one that was already so far out of date by the time I began working the BB10 Cordova, that it was of no use whatsoever. As a consequence, I fear that portions of this guide may also be obsolete by the time you need it. If so, let&#8217;s hope that this is because Blackberry has decided to fully support Linux, and a guide like this is no longer needed at all.

Let&#8217;s get down to business then.

### Preflight Checklist

Before we begin, this guide makes some assumptions about you, the reader:

  * You have some idea of what an extension is and does, and moreover, why you want to write one.
  * You have a github account, and you have already forked the WebWorks-Community-APIs repository.
  * I am using Ubuntu 12.10, and you are (obviously) using some version of linux. Where things might differ between us, you can handle yourself.
  * You are working on a machine for which you have administrative rights.
  * You have a BB10 device with which to work. I am using the Dev Alpha C model myself.
  * Your device has the latest OS installed. 
      * You can get that here: [https://developer.blackberry.com/devzone/blackberry10devalpha/devalpha_update.htm](https://developer.blackberry.com/devzone/blackberry10devalpha/devalpha_update.html)
      * Note however that updating the device OS via the autoloader is only possible through a windows machine (at this time)
  * You have a Blackberry ID set up already. If you don&#8217;t, you can do so from your device directly, although you&#8217;ll need an internet connection.

## The Guide

### Step 1: Momentics Installation

  1. Download and install Momentics SDK from
  
    <https://developer.blackberry.com/native/downloads/>
  2. Go to the directory where you saved the binary, chmod it to be executable, and run it (as yourself, not as root)
  3. I recommend you use all the default settings, unless you have a good reason not to.
  4. Allow Momentics to run after the installation is complete. If you don&#8217;t, you can always start it from the terminal: ~/bbndk/qde (assuming defaults)
  5. On startup, it will attempt to find your device. Let if fail, and see Step 2. If you don&#8217;t have one, you can ignore this and always deal with it later.

### Step 2: Device Setup

  1. Turn on your device, and go to Settings->Storage and Access
  2. Set the USB connection to &#8220;Connect to Mac&#8221; (see image below)
  3. Go back to Settings->Security and Privacy
  4. Scroll all the way to the bottom and select Development Mode
  5. Turn on development mode (see image below) 
      * This requires the device password, which I suggest setting to something very simple while you work
      * Note that development mode automatically turns off when the device restarts, or after 2-3 days
  6. Connect the device via USB cable, and on Momentics click &#8220;Try Again&#8221;
  7. Enter the device password when prompted
  8. Install the recommended API level, and go get a coffee (this takes a while)
  9. If prompted about installing debug stuff, do so, but then **do not** click restart until it completes (see image below)
 10. Click restart, but don&#8217;t expect it to actually open again on it&#8217;s own.

<img alt="" src="http://ucosp.ca/wp-content/uploads/2014/02/jpw_USB.png" width="600" height="800" /><img alt="" src="http://ucosp.ca/wp-content/uploads/2014/02/jpw_DevMode.png" width="600" height="800" />

<img alt="" src="http://ucosp.ca/wp-content/uploads/2014/02/jpw_Wait_Here.png" width="800" height="600" />

### Step 3: More Momentics Setup

  1. Open Momentics: ~/bbndk/qde
  2. Go to the menu: Window->Preferences
  3. Choose Blackberry->Signing from the panel on the left
  4. Enter your Blackberry ID password and click &#8220;Get Token&#8221; which will make you actually sign in with your Blackberry ID
  5. Once successful, click &#8220;Create Certificate&#8221;. You should no longer see a warning at the top of the page.
  6. Exit Momentics.

### Step 4: Install Node.js

  1. If you aleady have this, then go to step 5, otherwise enter the following commands from the terminal:
  2. sudo apt-get install python-software-properties python g++ make
  3. sudo add-apt-repository ppa:chris-lea/node.js
  4. sudo apt-get update
  5. sudo apt-get install nodejs

### Step 5: Install Cordova

  1. sudo npm install -g cordova
  2. You may need to add /usr/local/share/npm to your $PATH, but I had no issues without doing this.

### Step 6: Clone the WebWorks-Community-APIs repo locally

  1. Make a directory where you want to put it. I made ~/UCOSP since I was doing this for the UCOSP.
  2. cd ~/UCSOP
  3. git clone git@github.com:your-git-username/WebWorks-Community-APIs.git 
      * where your-git-username is your username for github
      * Permission Denied? You need to add an RSA key to github. Follow this helpful guide: <https://help.github.com/articles/generating-ssh-keys>

### Step 7: Environment Variables

  1. cd ~/bbndk
  2. ls
  3. Notice the file &#8220;bbndk*.sh&#8221; (see image below). I found that actually running the script did not do as intended, but simply sourcing it was sufficient:
  4. source bbndk*.sh
  5. You **must do this every time** you open a terminal to work, so you might as well add line 4 to you .bash_profile or similar file.

<img alt="" src="http://ucosp.ca/wp-content/uploads/2014/02/jpw_bbndk_dir.png" width="800" height="600" />

### Step 8: Running the Template Sample App

  1. cd ~/UCOSP/W\*/BB10-\*/T*
  2. cordova create sample2
  3. copy the www folder in /sample to /sample2, and overwrite anything there
  4. cd sample2
  5. cordova platform add blackberry10 
      * This is most likely fail. If not, go buy a lotto ticket.
      * The easiest solution is to change ownership of ~/tmp to yourself instead of root, then try again.
      * If you find an alternative solution, please document it, and let us know.
  6. cordova plugin add ../plugin
  7. cordova run sample2
  8. Your device will eventually start and app called &#8220;Cordova3&#8221;
  9. Click &#8220;OK&#8221; on the Web Inspector popup
 10. Scroll down to see the test output from the app
 11. Congratulations, the hard part is over!

<img alt="" src="http://ucosp.ca/wp-content/uploads/2014/02/jpw_SampleApp.png" width="600" height="800" />

### What&#8217;s Next?

The sample app uses the Template plugin to make several different types of Javascript calls to the native-level C++ underneath. To make your own extension, copy the Template directory, and use it as a basis for your work. Read Template/README.md for more information. Good Luck, and Happy Coding.