---
id: 2579
title: Flight Sim meeting minutes March 2nd
date: 2010-03-02T18:28:58+00:00
author: Michael Man
layout: post
guid: http://ucosp.wordpress.com/?p=2579
permalink: /2009-2010/flightsim/2010/03/flight-sim-meeting-minutes-march-2nd/
categories:
  - FlightSim
---
**Time:**

Mar 2nd, 2010 1pm EST

**Attendance**

Michael, Lenny, Matthew, Sylvain, Godfrey, Jean

**Absence:** 

Diane

 ****

**General Update**

  * Diane and Lenny with try both breakdown bar and histogram to see which one works better

Conference information

  * Tuesday: Skype only
  * Thursday: by phone:
  * Conference ID: 4450146
  
    Local Dial-in number: 416-343-2610
  
    Toll-free Dial-in number: 1 866-251-2605

**Goals for Sprint 3:**

**_The general goal is to create a tutorial, like many others on TE, with our graphical indicator._**** __**

**_The tutorial will have an entry to open up a page with dials just for that tutorial (in the same page of the tutorial)._**

**Individual tasks:**

**Matthew:**

  * **·** **Peter will attend one of the Thursday meetings, code and video demonstration will be required******

Diane:

&#8211; modifying css inside indicator.js (relative sizing)
  
&#8211; fix dials:
  
&#8211; > 100 values not showing properly
  
&#8211; > 100 error handling modification
  
&#8211; missing space between the value of the dials and the unit
  
&#8211; tableDefinitions:
  
&#8211; use of canvas, configure themes, custom error messages, refresh configurations
  
&#8211; images:
  
&#8211; enhance images
  
&#8211; create an indicator that looks like a histogram where every column has its own value.  Used to show past values if we want to monitor in time.  Example) Show different values from different sources of I/O monitoring that represent something only if they are seen high at the same time.

Will work with Alan to set up the <span style="text-decoration:underline;">latest version</span> of WMD on the server

Note: there are some changes in xml format on the WMD, when a person tests his code on the server, he should make the change accordingly, it is up to you if you want to install the latest WMD or not(you may have to spend another 3 days on that, take the risk if you want)

Lenny

Decided to implement a break-down bar for comparing different monitor values   it will be something like this: <http://img.skitch.com/20100301-cfdsgwbtmym45rm849p3qxy8j.png>

Have done a simple version and integrated into TE dashboard
  
Godfrey & Michael:

  * Created tickets for the next deliverable
  * Michael has uploaded the videos
  * Godfrey has tailored the video into a smaller resolution
  * Godfrey has talked with Lenny about the dials
  * Michael is merging everyone’s code in the repository and create a release. So please make sure your code are all checked into your personal branch
  * Will work together on Friday
  * **value of Row locks vs table locks may not be directly used, will investigate**

Jean & Sylvain:

  * Pushed research further to get more metrics to monitor
  * Asked Diane to create an indicator that look like an histogram, something like this <http://media.techtarget.com/digitalguide/images/Misc/iw_histogram.gif>
  * Checked the code from S2 into repository
  * Will create tickets for the next deliverable

**Issues:**

  * Please use the category S3 in your tickets!

**Important upcoming deadlines:**

**Mar. 13rd 2010 &#8211; Videos of scenario tutorials**

  * Build panels to make it easier to diagnose problems:

Mar. 23rd 2010 &#8211; Draft available for feed back

  * Build a method to allow someone to test a person

Mar. 21st 2010 &#8211; Draft available for feed back