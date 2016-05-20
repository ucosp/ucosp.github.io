---
id: 1311
title: One Step Backward
date: 2009-11-15T23:07:38+00:00
author: evanbowling
layout: post
guid: http://ucosp.wordpress.com/?p=1311
permalink: /2009-2010/ingres/2009/11/one-step-backward/
categories:
  - Ingres
tags:
  - drupal
  - php
---
Sometimes it is hard to recognize when a problem can be best solved by starting over. Over the past few days I have been making a lot of configurations on Windows using something called &#8216;Windows Configuration-By-Forms&#8217;. You can start it by going to the command prompt(typing &#8220;cmd&#8221; in Start->Run) and typing the command &#8220;cbf&#8221;.

Well, after all was said and done I wasn&#8217;t able to load php pages consistently. I previously was able to connect to an Ingres database, but not return any successful queries. Looks like I set something incorrectly.

However, since my role in this is to perform testing and documentation this will offer me the chance to document each step as I start over with my PHP install.

ASIDE:
  
I have heard that is not advised to use PHP 5.3 with Drupal, but I figure I will stick with what I had for tonight at least and see if I can get back to where I was.

Settings:
  
Apache v2.2 (running under user, NOT as service)
  
PHP 5.3
  
IngresII 9.3