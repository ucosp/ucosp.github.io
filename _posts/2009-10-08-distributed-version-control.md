---
id: 942
title: distributed version control
date: 2009-10-08T01:13:33+00:00
author: Eric Henry
layout: post
guid: http://ucosp.wordpress.com/?p=942
permalink: /2009-2010/thunderbird/2009/10/distributed-version-control/
categories:
  - Thunderbird
---
My team has been using [Mercurial](http://mercurial.selenic.com/wiki/) as our version control system, and it is definitely pretty cool.

We have run into some interesting &#8220;problems&#8221; though.  Since the main Thunderbird repository is subversion, and we don&#8217;t have commit access, we have to [submit patches that are reviewed and then committed](https://wiki.mozilla.org/Thunderbird/ISPDB#Making_a_patch).  The real problem comes with branching, merging, and committing.

Long story made short (or the moral of the story) is that newbies shouldn&#8217;t push/pull Mercurial repos from each other.  If they do, you end up with a mess that can only be solved by starting a new repo, and making your changes to that&#8230;

If you want more details, just post a comment and I&#8217;ll hook you up.