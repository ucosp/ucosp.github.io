---
id: 2039
title: 'First Push: Mercurial'
date: 2010-01-17T05:34:38+00:00
author: alexandru
layout: post
guid: http://ucosp.wordpress.com/?p=2039
permalink: /2009-2010/mercurial/2010/01/first-push-mercurial-2/
geo_latitude:
  - 43.661717
geo_longitude:
  - -79.396736
geo_accuracy:
  - 689
geo_address:
  - university of toronto
geo_public:
  - 1
categories:
  - Mercurial
  - Sprint
  - Status
tags:
  - hg
  - Mercurial
  - python
---
During this Code Sprint we focused on a few improvements to Mercurial that make it easier and safer to use. Each of the tasks we worked on was scoped such that only one developer was needed, but this gave everyone a chance to dive head-first into the Mercurial codebase at their own pace. For some (myself included) this is also the first serious project in Python, and these two days were a great opportunity to ask lots of questions.

We&#8217;re well on our way implementing support for using git sub-repositories, interactively editing Mercurial&#8217;s config files (`.hgrc`), cache annotations, auto-merging `.hgtags`, matching wildcards when converting from a different source-control system to Mercurial, and preventing users from using files whose names differ only in case (i.e. `filename` and `FileName`).

We&#8217;ve also discussed the harder problems we&#8217;re attempting over the next few months, namely fixing the way Mercurial handles history for large file renames, improving the way very large files are being stored, and improving `hg serve` output. And we&#8217;re sure there will be plenty more to do.

If you want to take a look at what&#8217;s going on in our world, please check out the  [UCOSP FogBugz](http://ucosp.fogbugz.com "UCOSP FogBugz") install and log in with `Guest/anonymous`.