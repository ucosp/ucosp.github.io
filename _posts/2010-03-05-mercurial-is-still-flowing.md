---
id: 2610
title: Mercurial is still flowing
date: 2010-03-05T02:54:04+00:00
author: Anton Markov
excerpt: |
  Status update: we've made progress in closer integration between bfiles and core Mercurial commands, a tool to "bfilesify" a Mercurial repository, and further work on the caseguard extension.
layout: post
guid: http://ucosp.wordpress.com/?p=2610
permalink: /2009-2010/mercurial/2010/03/mercurial-is-still-flowing/
categories:
  - Mercurial
  - Status
---
In Mercurial land, we&#8217;ve made progress in closer integration between bfiles and core Mercurial commands, a tool to &#8220;**bfile**sify&#8221; a Mercurial repository, and further work on the caseguard extension. More details below.

Due to various scheduling conflicts, we did not have a status meeting last week. This week the meeting happened on Wednesday at 9pm EST. We&#8217;ll be back to Thursdays at 6:30pm EST starting next week.

Chat transcript: <https://ucosp.fogbugz.com/default.asp?W38>

Status reports for two weeks:

  * [February 25th](https://ucosp.fogbugz.com/default.asp?W35)
  * [March 3rd](https://ucosp.fogbugz.com/default.asp?W36)

Closer bfiles integration: as I&#8217;ve discussed in a [previous post](http://ucosp.wordpress.com/2010/01/29/mercurial-progress-report-week-4/ "Week 4 status report introducing bfiles"), bfiles is an extension to store history of big and binary files outside the repository. Currently ther bfiles extension has its own set of commands: &#8216;hg bfstatus&#8217; analogous to &#8216;hg status&#8217;, &#8216;hg bfadd&#8217; analogous to &#8216;hg add&#8217;, etc. We want to integrate them into the core commands like &#8216;hg status&#8217;.

While I spent my time discussing auto-status integration and debating the proper way to do it, Tessa and Wendy made significant progress on auto-put, auto-update, and auto-refresh. We are ready to try using and testing the parts together before making them ready for submission (as individual patches/branches).
  
[Edit 3/5/2010: removed confusing wording about &#8220;combining into a single patch&#8221;]

Paul has taken up the torch on a much-needed extension we call &#8216;bfilesify&#8217; which would take a regular repository and convert it to using bfiles where appropriate. This is an exciting project which should greatly ease the transition to bfiles.

Last but not least, Alex has been polishing up caseguard and improved its performance to the point where the impact on speed from using caseguard is negligible. Caseguard has also become a somewhat regular topic on the mercurial mailing lists &#8211; a good indication that it sees real use.