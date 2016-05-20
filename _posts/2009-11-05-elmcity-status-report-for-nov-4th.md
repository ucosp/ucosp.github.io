---
id: 1211
title: ElmCity Status Report for Nov 4th
date: 2009-11-05T16:16:38+00:00
author: Diane Tam
layout: post
guid: http://ucosp.wordpress.com/?p=1211
permalink: /2009-2010/elmcity/2009/11/elmcity-status-report-for-nov-4th/
categories:
  - ElmCity
  - Status
tags:
  - ElmCity
---
**Nikita**

Status:
  
+documenting and testing remote.py, batch.py (this leaves us with no &#8220;big&#8221; modules untested, rotate.py and event.py can
  
be done quickly later on).
  
+ timezone had to be revisited and changed a bit (timezone\_source, timezone\_dest), and together with other little things
  
we officially announced the new features to the community

Roadblocks:
  
&#8211; I&#8217;ve been sick for the past couple of days, so things are moving a bit slower for me than usual.
  
It&#8217;s not a real roadblock, just letting everyone know why I was semi-silent since Friday.
  
&#8211; we need to adopt development / stable scheme on the web server, Jory what&#8217;s the status on that one?
  
&#8211; tests are not working for one of the plugins and for the integration testing, Meghan, Jack what&#8217;s the status
  
on those ones? It&#8217;s not a major roadblock per se (the problems are with the test code itself, not with the
  
project&#8217;s code), but it&#8217;d be nice if they worked.

Next Steps:
  
I want to concentrate on the patterns and generalized plugin from now on, spending much less time
  
on the service as a whole, after all we have a stable version in the repos right now and the next
  
big step is the generalized plugin.

**Diane**

Status:
  
&#8211; Refined a generic plugin that can parse some pages successfully.  Latest plugins have been delivered to google code repository.
  
&#8211; Continually working towards generalizing the scraper to scrape multiple sites.
  
&#8211; Documenting patterns through blog and tester.  Latest post in regards to plugin and patterns can be found here: <a title="Patterns and thoughts continued" href="http://dianetam.com/dev/blog/2009/11/05/patterns-and-thoughts-continued/" target="_blank">http://dianetam.com/dev/blog/2009/11/05/patterns-and-thoughts-continued/</a>

Roadblocks:
  
&#8211; Work, classes.

Next Steps:
  
&#8211; Continue to scrape and document patterns found from event sites.
  
&#8211; Establish a more complete analysis of the patterns found from the fuse-cal parsed pages as well as the sample pages curators have pointed to.
  
&#8211; Divide the list according to the patterns found and manage the lists (ie. through Delicious tags).
  
&#8211; Populate that dictionary for all our targets plus the ones the curators have added to our list.
  
&#8211; Build a tester that will accept the various patterns and extract appropriate information from them