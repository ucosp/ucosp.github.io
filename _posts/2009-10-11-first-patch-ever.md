---
id: 958
title: First Patch Ever.
date: 2009-10-11T20:22:47+00:00
author: nidol
layout: post
guid: http://ucosp.wordpress.com/2009/10/11/first-patch-ever/
permalink: /2009-2010/uncategorized/2009/10/first-patch-ever/
categories:
  - Thunderbird
  - Uncategorized
tags:
  - ISPDB
---
First Patch Ever.

Once my pending patch has been checked into the source tree, I will become a member of the open source community. It doesn&#8217;t look like much but it does fix a problem. I take heart from Richard Feynman who said, &#8221; No problem is too small or too trivial if we can really do something about it.&#8221;.  Here is a few things I learned:

1. Svn needs a better way to manage patches because pending ones causes a mess. To keep from mangling my patch, I ended up having to checkout another copy to code with. If anyone has a better solution please tell me.

2. Stand on other people&#8217;s shoulders. We borrowed a custom test runner to integrate the nose test framework into django during the code sprint (Thanks Jeff!). Then we discovered that he maintains a version of it on github so now we point to the source and save ourselves maintence/installation issues.

3. People on IRC are really nice. I needed help with my patch so I hopped on IRC (mozilla/education). It was nice to have someone who knew a lot about coding and ISPDB (David Ascher) take the time to thoroughly discuss the issues.