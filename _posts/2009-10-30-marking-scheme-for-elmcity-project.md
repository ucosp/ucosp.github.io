---
id: 1154
title: Marking Scheme for ElmCity project
date: 2009-10-30T23:23:24+00:00
author: Nikita Pchelin
layout: post
guid: http://ucosp.wordpress.com/?p=1154
permalink: /2009-2010/elmcity/2009/10/marking-scheme-for-elmcity-project/
categories:
  - ElmCity
---
**Mark Breakdown**

**1. Individual (50%)**

a) **40%** &#8211; participation:

  * **20%** code contributions
  * **10%** discussions on friendfeed and google code wiki throughout the term
  * **10%** weekly punchlines and how they were met (trackable through the &#8220;status&#8221; portion)

b) **10%** &#8211; written component

**2. Team (50%)**

a) **30%** Features and Functionality:

  * all the existing functionality up-to-date (plugins, events filtering, timezones management) still works as expected (test don&#8217;t fail), existing bookmarks on delicious produce valid iCal feeds
  * generalized parser that can **at least** recognize a minimum set of information for the event (date & time, title, and a link) on each of the pages listed <a href="http://friendfeed.com/elmcity/92ef3b61/hey-everyone-team-over-in-elmcity-development" target="_blank">here</a>. If for some reason some of the page(s) are odd and cannot be parsed by the generalized plug-in, we must opt-out for completing a site-specific plug-in. If time permits, (outside 30%) we are targeting pages on <a href="http://blog.jonudell.net/2009/07/07/strategic-choices-for-calendar-publishers/" target="_blank">here</a> and too
  * product has to be ready to be shipped. That is, we have to have a document that describes all the third party libraries (and software) one may need to yank a fresh copy from google code and start working with the code. We can include general steps (i. e. have mysql, phpmyadmin installed and working), but whatever concerns the project itself must be specific (i. e. what file do I edit to change the location of calendar folder?)

b) **10%** system has a clear documentation (comments inside the files, high-level description of the system) that could potentially allow other people to contribute to the project. Tests has been implemented (unit and integration) and run smoothly.

c) **10%** written report + youtube presentation of the service, that describes what work has been done through out the term, demonstrates the abilities of the project, touches on the future of the project (i.e. if we were to continue, what are things that are missing and that we&#8217;d wanted to implement in the future)