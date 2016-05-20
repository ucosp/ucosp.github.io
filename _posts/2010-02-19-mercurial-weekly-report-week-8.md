---
id: 2302
title: Mercurial Weekly Report (Week 8)
date: 2010-02-19T16:19:42+00:00
author: q6yang
layout: post
guid: http://ucosp.wordpress.com/?p=2302
permalink: /2009-2010/mercurial/2010/02/mercurial-weekly-report-week-8/
categories:
  - Mercurial
  - Status
---
We continued our work on bfiles and improving our patches this week.

**Patches:**

  * cedit (paulitex): 
      * Submit unit test and rege fix for iniparse
      * Documentation for credit

  * tagmerge(Wendy): 
      * Use tag.py functions to read tags
      * Changed the merge algorithm
      * Debugging writing tags problem

  * convert (Tessa): 
      * Tested standard mercurial matcher
      * Refactored filemapper to use the mercurial match

  * caseguard (alexandru): 
      * Removed the protection for \`hg rm&#8217;
      * Code clean-up/polish

**bfiles:**

  * auto-status(antmar): implemented and submitted the initial version (wraps &#8220;hg status&#8221; command)
  * auto-put(Tessa): read through more code about it and revisited the proposal
  * auto-refresh & auto-update (Wendy): created detailed proposal on the mailing list and discussed about the proposal
  * bfiles HTTP upload(alexandru): started investigate this issue

We further discussed the problems we met this week and plan to finish the patches and submit a working code draft for bfiles command integration.

Details are in [IRC meeting](https://ucosp.fogbugz.com/default.asp?W6) and [status report](https://ucosp.fogbugz.com/default.asp?W34) .