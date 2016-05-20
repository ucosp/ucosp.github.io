---
id: 2150
title: Eclipse4Edu Meeting Minutes
date: 2010-01-23T01:35:20+00:00
author: Brenda Sadoway
layout: post
guid: http://ucosp.wordpress.com/?p=2150
permalink: /2009-2010/eclipse4edu/2010/01/eclipse4edu-meeting-minutes/
categories:
  - Eclipse4Edu
tags:
  - meeting minutes
---
The meeting was held at 2:00 EST today and all members were present.

**Brenda**

&#8211; Working on hiding packages from the user

&#8211; Buttons are easily hidden

&#8211; Has been able to identify which elements of the package explorer are in fact packages, but is stuck on reworking the hierarchy so that the view skips over the package level

**Cory**

&#8211; Working on hiding menus and toolbars

&#8211; Tried making his own RCP app because it seems this might be the best approach to get rid of unneeded menus and toolbars

**Miles**

&#8211; Is going to take on the task of separating the UI and actual creation of classes, as per Wayne’s comments in the mailing list and in Bug 300275

&#8211; Will send Cory links related to hiding menus and toolbars, which may be useful

**Java Lite Debugger**

&#8211; Discussed the idea of a Java Lite debugger

&#8211; Cory put forward the idea of creating our own editor that pulls in the needed functionality from the Eclipse editor, and tailoring it to work as a simple debugger simultaneously (that is, it always debugs).  For example, if it throws an error on execution, it goes into debug mode, much like on an uncaught exception, and of course it would stop at breakpoints

&#8211; The idea is to make debugging useful and intuitive right from the beginning, and to have everything accessible in the editor