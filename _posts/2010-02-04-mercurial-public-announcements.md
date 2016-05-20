---
id: 2234
title: 'Mercurial: Public Announcements'
date: 2010-02-04T19:50:34+00:00
author: alexandru
layout: post
guid: http://ucosp.wordpress.com/?p=2234
permalink: /2009-2010/mercurial/2010/02/mercurial-public-announcements/
geo_longitude:
  - -123.245837
geo_latitude:
  - 49.265637
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
All of us on the Mercurial team have submitted extensions and patches to the devel mailing list this week:

  * Anton&#8217;s _cache annotations_ extension ([list announcement](http://selenic.com/pipermail/mercurial-devel/2010-February/018313.html))
  * Paul&#8217;s _cedit_ configuration editor extension ([list announcement](http://selenic.com/pipermail/mercurial-devel/2010-February/018318.html))
  * Tessa&#8217;s _convert_ patch, to support glob excludes ([list announcement](http://selenic.com/pipermail/mercurial-devel/2010-February/018338.html))
  * Alexandru&#8217;s _caseguard_ case-fold collision prevention extension ([list announcement](http://selenic.com/pipermail/mercurial-devel/2010-February/018368.html) | [blog post](http://mrtoto.net/post/370905475/caseguard-a-mercurial-extension))
  * Wendy&#8217;s _tagmerge_ extension for merging .hgtags ([list announcement](http://selenic.com/pipermail/mercurial-devel/2010-February/018387.html))

The feedback&#8217;s been great so far, as have the bug reports (which means at least a few people tried out what we made). We&#8217;re planning on moving on to [new things](https://ucosp.fogbugz.com/default.asp?W19) in the coming weeks, though of course we&#8217;ll have to maintain our extensions from now until forever. It was a good week in the Mercurial camp.

## WEEKLY STATUS MEETING

During our regularly scheduled weekly meeting, we decided to engage with the Mercurial community at large, so we moved from our regular place on #ucosp-mercurial to the main Mercurial IRC channel, #mercurial (both on Freenode, details on our [Communications](https://ucosp.fogbugz.com/default.asp?W6) page). The discussion revolved mostly around bfiles, an extension all of us are working on currently. Bfiles allows Mercurial users to store their large binary files in remote locations, and as we&#8217;re improving the existing code-base, certain decisions need to be made before development can move forward. The complete IRC log for the meeting [is available](https://ucosp.fogbugz.com/default.asp?W28) as usual, and a more detailed breakdown of what everyone&#8217;s working on can be found on our [weekly journal page](https://ucosp.fogbugz.com/default.asp?W13).