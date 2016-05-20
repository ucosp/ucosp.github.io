---
id: 2693
title: 'mercurial # the end if nigh'
date: 2010-03-26T20:41:36+00:00
author: alexandru
layout: post
guid: http://ucosp.wordpress.com/?p=2693
permalink: /2009-2010/mercurial/2010/03/mercurial-the-end-if-nigh/
geo_latitude:
  - 49.265637
geo_longitude:
  - -123.245837
geo_accuracy:
  - 0
geo_address:
  - 2125-2199 Wesbrook Mall, Greater Vancouver A, BC, Canada
geo_public:
  - 0
categories:
  - Mercurial
  - Status
---
For some of us on the Mercurial crew next week is the closing chapter of the UCOSP adventure. Tessa, Wendy and Anton from Waterloo will be finishing their term, and with that their contributions to Mercurial as part of the program. That&#8217;s not to say they&#8217;ll be done with Mercurial for good—the general consensus is that we all had a great time. Paul and myself still have until mid-April to get the remainder of our work submitted.

For the last couple of weeks we&#8217;ve all been focusing on bfiles, the big/binary file extension for Mercurial. For the most part, the functionality that&#8217;s been added is to automate certain functions so that the user doesn&#8217;t have to remember to do so:

**Tessa** finished up autoput, including tests for the feature. She&#8217;s also submitted a few more changes for her globexclude patch.

**Wendy** worked on autorefresh and autoupdate for bfiles, as well as some final tweaks for her tagmerge extension.

**Anton** polished up autostatus for bfiles and began work on extended status support.

**Paul** has been working on bfilesify, an extension to convert a regular Mercurial repository to a bfiles one. This means all large binary files get detected and plugged into bfiles, with the history accurately maintained.

**Alexandru** worked on supporting HTTP PUT for bfiles, so that users can push their large files to remote repositories via HTTP (currently, only SSH is supported). Additional work went into caseguard to provide a feature that allows users to check an existing repository for filename issues. Alexandru also apologizes for talking in the 3rd person for this section, it was done in the interest of post formatting.

More information available from our weekly [Wiki status page](https://ucosp.fogbugz.com/default.asp?W41) and the [IRC log](https://ucosp.fogbugz.com/default.asp?W43).