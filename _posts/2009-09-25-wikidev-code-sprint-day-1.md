---
id: 811
title: WikiDev Code Sprint (Day 1)
date: 2009-09-25T20:56:09+00:00
author: Holly Becker
layout: post
guid: http://ucosp.wordpress.com/?p=811
permalink: /2009-2010/wikidev/2009/09/wikidev-code-sprint-day-1/
categories:
  - WikiDev
---
The WikiDev team met this morning for the first time, and did the usual round of introductions, learning everyone&#8217;s names &#8211; and, in Botlhale&#8217;s case, pronunciations.  Testing databases were setup, and the SVN repository was populated with existing code, giving us lots of stuff for playing around and testing.  As a team, we decided on the architecture of the system, debating the virtues and vices of a couple of options.

As before, we split up into three teams by university:  SFU with Holly and Alex, University of Waterloo with Owen and Eric, and University of Victoria with Botlhale.

SFU installed Eclipse/Flex Builder, and configured Subclipse to work properly.  We also reviewed existing code from a similar application to see how it worked, and how we could modify it.  Brendan, a veteran on the project, gave a summary of the existing system, which consists of two databases, a wiki, and lots of meta-data to display.  With Botlhale and Brendan&#8217;s help, we drafted a data format for transferring data between parts of the project.

UWaterloo was hard at work understanding how the existing XMI parser works, and how to modify it to suit our current needs.

UVic started learning PHP, and looked at the existing MediaWiki extension code for producing XML.  He also helped SFU decided on an XML data format, and learned how the existing system worked.