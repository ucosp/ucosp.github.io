---
id: 1120
title: ElmCity Status Report for Oct 28th 2009
date: 2009-10-29T02:39:58+00:00
author: Diane Tam
layout: post
guid: http://ucosp.wordpress.com/?p=1120
permalink: /2009-2010/elmcity/2009/10/elmcity-status-report-for-oct-28th-2009/
categories:
  - ElmCity
  - Status
---
**Nikita**

Status:
  
&#8211; AM/PM problem for librarything fixed, tests added
  
&#8211; timezone, we have a solution and it has been implemented and is out there for testing, calling remote like this:
  
http://elmcity.cs.toronto.edu/remote/?url=http://www.myspace.com/cartel&filter=Portland&tz=atlantic
  
generates a VTIMEZONE in the calendar file. We support standard tzid from Olson db, and we map all the
  
windows timezones that elmcity provides us with to the existing tzids.
  
&#8211; pluginFinder.py, icwWriter &#8211; written documentation, unit tests
  
&#8211; moved views.py code into a separate file, and made views.py call it from there (this is to enforce independence from django)
  
&#8211; extending web-interface &#8211; I have not done much, just changed how AJAX communicates with python (XML now), so that
  
if we eventually look at extending it, it will be easier, plus that killed the last hard-coded reference in javascript code (domain name)

Roadblocks:
  
none

Next Steps:
  
&#8211; I have not seen any work done on #2 as was agreed on Friday&#8217;s meeting, this is an important issue that is kinda holding
  
us back. If there will be no change by tomorrow&#8217;s afternoon I am reassigning this ticket to myself and most probably closing
  
it by tomorrow&#8217;s evening
  
&#8211; documenting and testing remote.py, batch.py (this leaves us with no &#8220;big&#8221; modules untested, rotate.py and event.py can
  
be done quickly later on).
  
&#8211; I&#8217;ve been thinking of coming up with an approach of looking at HTML pages and finding events(here:
  
http://nikitapchelin.wordpress.com/2009/10/25/patterns/)  My idea is to actually
  
try and look for dates first, and then look and compare where structure-wise those dates are located. From that information
  
it might be possible to figure out which structured blocks represent events. I actually started working on a little script
  
that strips useless things from HTML and tries to find events. I want some sort of discussion, mainly to see if this
  
direction is worth moving into. If indeed so, I would like to continue exploring this way throught the week and coming up
  
with a script that will attempt to analize HTML pages this way.

**Diane**

Status:
  
&#8211; Completed some site specific scrapers for fuse-cal parsed pages, specifically with <table> structured event sites.
  
&#8211; Continually working towards generalizing the scraper to scrape multiple sites.
  
&#8211; Documenting patterns through blog and tester.

Roadblocks:
  
-Work, classes.

Next Steps:
  
&#8211; Continue to scrape and document patterns found from event sites.
  
&#8211; Establish a more complete analysis of the patterns found from the fuse-cal parsed pages as well as the sample pages curators have pointed to.
  
&#8211; Divide the lists according to the patterns found and manage the lists through Delicious tags.
  
&#8211; Build a tester that will accept the various patterns and extract appropriate information from them.

**Jory**

Roadblocks:
  
&#8211; Assignments and midterms.

Next Steps:
  
&#8211; Go through all the communication channels from last week, and to try to summarize the state of the project in a blog post. I will combine that with the feature requests put forth by the users on FriendFeed in an attempt to figure out both where we are at, and what our endgame looks like. I&#8217;ll also be adding the features requested by the users as items to our issue tracking system.

**Meghan**

Status:
  
&#8211; I completed the librarything tests and committed them along with corresponding files earlier this week.  Nikita has already pointed out the page reformatting check fails on his computer so I need to look into those two functions more this week and come up with a better solution.

Roadblocks:
  
&#8211; Other classes, projects and tests.
  
&#8211; Ran into some hg issues.  I commented out the reformatting tests earlier today and commit them so test_all.py wouldn&#8217;t fail.  I tried to commit them but I kept getting a 403 error when my username and password were correct.  I need to look into this further.

**Jack**

Status:
  
&#8211; I got the zombies issue resolved, couple more things I&#8217;d like to do on that front though.  Nikita mentioned that one of the integration tests is broken from this update, so I&#8217;m going to resolve that tonight or tomorrow.  I&#8217;d like to do a little more testing of everything tomorrow if I have time as well.

Roadblocks:
  
&#8211; Classes/other projects due, job interview.