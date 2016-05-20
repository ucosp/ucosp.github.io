---
id: 1036
title: Punchlines Oct 19-25 ElmCity team
date: 2009-10-21T16:59:46+00:00
author: Nikita Pchelin
layout: post
guid: http://ucosp.wordpress.com/?p=1036
permalink: /2009-2010/elmcity/2009/10/punchlines-oct-19-25-elmcity-team/
categories:
  - ElmCity
---
**Sarah**

Status:
  
&#8211; The project I was working on got canned, so I&#8217;m trying to get reacquainted with the core codebase
  
&#8211; Also trying to understand the intended goals and power structure of this project better so I don&#8217;t waste more work. This entails some discussion, new use of the bug tracking system for laying out goals, and group formulation of user stories (to be finished at this Friday&#8217;s meeting)

Roadblocks:
  
&#8211; Midterms
  
&#8211; If we write user stories as a group on Friday without Jon, how do we make sure he clears each one, and what do we do if he rejects many of them? I&#8217;m concerned this could make Friday&#8217;s meeting less useful than it otherwise would be. Alternatives: Solicit a comprehensive description of what Jon thinks are acceptable high-level goals before Friday and refine at the meeting, adding no additional ideas so we don&#8217;t stray from spec, or, better, have Jon come to the meeting if possible.

Next Steps:
  
&#8211; Write documentation
  
&#8211; Write tests, and add any bugs I discover to bug tracker
  
&#8211; Choose all future tasks from the bug tracker for better directed work
  
&#8211; Turn agreed-upon and authorised user stories into a series of milestones specified in the bug tracker, choose one as a milestone for one or two weeks from now
  
&#8211; Use user stories generated plus group discussion to formulate marking scheme

**Nikita**
  
Status:
  
&#8211; http://elmcity.cloudapp.net/services/frenchThings/html (different types of feeds showing up!)
  
&#8211; removed all relative links in the code, which now allows us to check out code and develop locally much easialy
  
&#8211; added filtering ability to the service (url=&#8230;&filter=Montreal)
  
&#8211; rewrote librarything plugin to use RSS instead of HTML when parsing events
  
&#8211; myspace (fixed issue #36, choking on certain pages with missing location information)
  
&#8211; tests: wrote tests and docuemnted myspace, librarything, database.py, added test_all.py (that creates a test suite from available test modules and runs them all)
  
&#8211; wrote initial batch module (batch.py)
  
&#8211; started two wiki pages (http://code.google.com/p/elmcity/w/list) one for &#8220;how to write a plugin&#8221;, the other one describing the general look of the system.
  
&#8211; other little things

Roadblocks:
  
&#8211; none
  
Next Steps:
  
&#8211; looking and coming up with the solution for the timezone problem (as per http://friendfeed.com/elmcity-development/735c49eb/problem-with-librarything-approach) and
  
AM/PM problem (as per http://friendfeed.com/elmcity-development/abbbced4/paris-est-belle)
  
&#8211; pluginFinder.py, icwWriter &#8211; documentation, unit tests

not-so-important:
  
&#8211; move views.py code into a separate file, and make views.py call it from there (this is to enforce independence from django)
  
&#8211; extending web-interface
  
&#8211; more things if time permits!

**more to come**