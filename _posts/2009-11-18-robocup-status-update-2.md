---
id: 1338
title: Robocup status update
date: 2009-11-18T06:07:16+00:00
author: Chani
layout: post
guid: http://ucosp.wordpress.com/?p=1338
permalink: /2009-2010/robocup/2009/11/robocup-status-update-2/
categories:
  - RoboCup
  - Status
---
alex:
  
-has been trying to improve passing by having the kicker shout out where the ball is going, but the other players don&#8217;t always hear it
  
-will try other ways to improve passing

chani:
  
-implemented ball and player decay
  
-found out that the code for updating object positions was never being called and fixed that
  
-is working on vision optimization
  
-improved the debug viewer a bit more
  
-may also experiment with changing minimum-confidence values

ioana:
  
-found a passing bug, and is looking into interception problems
  
-was trying to get the new human controller to work, no luck
  
-is working on ball interception

patrik:
  
-was working on merging all the branch stuff into trunk
  
-hardware issues corrupted all his work, so he has to redo it

yulia:
  
-found a problem with vision &#8211; only the first two flags are being used to determine position
  
-was going to fix it but ended up in hospital instead
  
-wrote a small gui for starting teams and server
  
-started modifying the on_see function
  
-rewrote sexpparser and made it faster