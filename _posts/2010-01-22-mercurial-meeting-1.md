---
id: 2131
title: Mercurial Meeting 1
date: 2010-01-22T05:22:30+00:00
author: Anton Markov
layout: post
guid: http://ucosp.wordpress.com/?p=2131
permalink: /2009-2010/mercurial/2010/01/mercurial-meeting-1/
categories:
  - Mercurial
  - Status
---
Our team had our first remote meeting today (Thursday). We covered progress made this week, discussed obsticles, and plans for the near future. A quick summary follows. You can find the whole transcript at: <https://ucosp.fogbugz.com/default.asp?W10>

Progress:

  * paulitex: a couple of new features/extensions for config-editor extension. Only a couple more TODOs left. Looking for code reviews.
  * alexandru: worked on caseguard extension to support &#8216;hg rm&#8217;. Still needs to address code review feedback.
  * antmar: not much new work on cache-annotations, but did go and reviewed paulitex&#8217;s config-editor work. Need to add support for case-neutral names in the annotations cache.
  * Tessa: solicited feedback about using shell-globs (wildcards) to exclude files during conversion. We came to a consensus, and Tessa is in the process of testing the changes.
  * wendyY: writing tests for tagmerge this week following a small skirmish with some biological viruses (a cold).

Looking forward:

  * bmp: once we are ready to submit to mercurial-developers list, we need to learn how to package up our patches. When our current tasks have been completed and submitted, start attacking the bfiles extension. 
      * For reference: bfiles is an extension to improve the way Mercurial handles large binary files in its repositories.
  * paulitex, alexandru: will attempt pair-programming on bfile issues
  * antmar, Tessa, wendyY: take ownership of one issue each, but work together as much as possible on all the issues. 
      * We&#8217;ll report on how this works out.

We&#8217;ll be having weekly meetings &#8211; same time, same place, similar agenda:

  * What: UCOSP Mercurial weekly meeting
  * When: Thursdays at 6:30pm EST / 3:30pm PST.
  * Where: #ucosp-mercurial on freenode.net
  * Logs: <https://ucosp.fogbugz.com/default.asp?W6>