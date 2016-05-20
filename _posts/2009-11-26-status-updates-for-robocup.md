---
id: 1466
title: Status updates for Robocup
date: 2009-11-26T03:10:53+00:00
author: kyokko
layout: post
guid: http://ucosp.wordpress.com/?p=1466
permalink: /2009-2010/robocup/2009/11/status-updates-for-robocup/
categories:
  - RoboCup
  - Status
---
We had our [meeting](http://chani.ca/robocup/minutes/22_nov_minutes.rtf) on Sunday, November 22. Here is what the team had been up to:

Alex

&#8211; worked on passing, now it takes into account players from the opposit team

&#8211; it is hard to make 100% accurate passing because of the noise added to the measurements

Next task:

&#8211; work on interception as it is related to passing

Chani

&#8211; fixed code so that now players are using data from the current tick

&#8211; fixed a bug in the debug ui

Next task:

&#8211; continue debugging

Ioana

&#8211; worked on dribbling

&#8211; found bug that causes a player to be stuck near the ball not making any actions

possible reason is that position of the player and the ball is not update properly

Next task:

&#8211; continue working on dribbling

Yulia

&#8211; rewrote chunk of code responsible for parsing the s-expressions from the server

&#8211; slightly improved the accuracy of statistics computed from the server data

but it seems that there is not much we can do to make it better because of the

server restrictions

Next task:

&#8211; continue debugging

Patrik

&#8211; did a merge of code from the dt branch into trunk

Next task:

&#8211; debugging kick/dribbling