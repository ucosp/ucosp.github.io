---
id: 1033
title: Robocup Status Update
date: 2009-10-21T16:10:13+00:00
author: ioanaiv
layout: post
guid: http://ucosp.wordpress.com/?p=1033
permalink: /2009-2010/robocup/2009/10/robocup-status-update/
categories:
  - RoboCup
---
**Alex**

Status:
  
&#8211; Tried to tweak to Java client to produce data file for Decision Tree. However, it was cancelled since we might not need it due to Yulia&#8217;s work to parse server log file.
  
&#8211; Training a goalie with the human controller to produce a convincing data file.

Next tasks:
  
&#8211; Testing Yulia&#8217;s log parser.
  
&#8211; Finding the right parameters to build Decision Tree.

Roadblocks:
  
&#8211; It is very difficult to get a high-quality of training data for building a good Decision Tree. Training a goalie properly with the human controller is very hard as we can&#8217;t move it as fast as we want.**
  
** 

**Yulia**

Status:
  
&#8211; Finished logparser for .rcg and .rcl log files. Now it extracts all attributes that user wants and dumps them all into .data file that can immediately be used for c4.5
  
&#8211; Made some progress on compiling the human controller

Next Tasks:
  
-more work on decision trees

Roadblocks:
  
-None
  
**
  
Chani and Patrick**

Status:
  
&#8211; Worked on adding meta-actions: the action class can support multi-tick actions now

Next tasks:
  
&#8211; start implementing some of the actions in the Actions class

Roadblocks:
  
&#8211; None

**Ioana**

Status:
  
&#8211; Made some changes to the debug gui
  
&#8211; Looked into the neckrotator algorithm used by the Java client

Next task:
  
&#8211; Start implementing neck rotator
  
&#8211; Look into vison quality mechanism that Chani mentioned

Roadblocks:
  
-None