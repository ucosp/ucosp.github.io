---
id: 2402
title: 'alexandru&#039;s Half-Time View'
date: 2010-02-26T01:31:35+00:00
author: alexandru
layout: post
guid: http://ucosp.wordpress.com/?p=2402
permalink: /2009-2010/mercurial/2010/02/alexandrus-half-time-view/
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
## warm-up

I&#8217;ve used open-source software for the last 7 years (which <del>is</del> _feels like_ a blip in Internet time). I was aware since the beginning that these projects thrive on contributions from people all over the world. And I knew that these tools had bugs and had roadmaps with desired features waiting on some developer to tackle. But before UCOSP I&#8217;ve never made a solid contribution to anything. I always imagined expert programmers are the only ones that have a business getting involved in these projects and submitting patches and extensions. So I stayed on the sidelines for the most part, always saying I&#8217;ll do it later, when I got better at programming.

When UCOSP started, I was thrilled to be working on the Mercurial project. I was also thrilled to finally have the time to learn Python, and terrified by not really knowing any. I had my doubts, early on, about being able to get something decent done by the end of April. This wasn&#8217;t the first time I dived head-first into something of the sort (having completed 5 internships at various software outfits during my student career), but it felt different. It was going to be out in the world for people to use. I was finally working on an open source project, planning on contributing something I knew was needed.

Guess what? It&#8217;s going great! Over the past years I kept hearing that failing is not a bad thing, that if you don&#8217;t get it right the first time the World won&#8217;t implode. I&#8217;ve learnt that failure comes more often from the desire to be perfect than from the work itself, because perfection is the enemy of productivity, and over-engineering is something we&#8217;re all very prone too. So I made bite-sized goals and I&#8217;ve incrementally built [caseguard](http://hackd.net/projects/caseguard "caseguard"), my Mercurial extension that&#8217;s meant to help developers avoid filename collisions (on case-insensitive filesystems) and the feedback so far has been good. The Mercurial devel mailing list has been invaluable for both feature recommendations and help with the existing design, and the UCOSP mentor, [Benjamin Pollack](http://bitquabit.com) has been similarly patient with us.

## sideline

Acquaintance to how open source works is an indispensable experience, especially for students, because it&#8217;s so different from anything else we&#8217;re normally exposed to. All great software, whether open source or not, is built because someone needs it. Often times students and junior developers don&#8217;t get an opportunity to pursue their ideas inside a project because the requirements are either filling up the entire course time, or the senior developers have already outlined the things that need to get done. But with open source (and, by extension, UCOSP) we get to own our code and take it in whichever direction we feel it should go. Community feedback can be a driving force, but it&#8217;s not law. Learning how to prioritize, which features are important and which nice-to-have ones you should delay until a time they&#8217;re actually needed, quieting the inner voice that wants to keep adding things because some believe that more is better, these are all skills that matter greatly in software development. Sometimes, they might decide a project&#8217;s success more than the pure programming prowess of the developers involved.

I wish I started contributing to open source earlier, but it&#8217;s never too late. The biggest failure comes from not trying at all; anything else is already better. My experience in UCOSP so far proves my point, and I hope that&#8217;s true for everybody across all teams this term. I hope UCOSP-like courses become the norm in Computer Science/Engineering programs, because they help a developer&#8217;s education once all the theory has been absorbed throughout the program years.

## second half

For the second part of the term I&#8217;m going to continue work on caseguard, targeting inclusion in the Mercurial distribution for 1.6 (targeted release July 1st). It may be an extension included in the core distribution or it may be part of the actual tool itself (over IRC, the Mercurial project lead Matt Mackall suggested I submit a patch to see how it would work in core) and that&#8217;s all very exciting. Python is a very elegant language and I&#8217;m liking it the more I learn it, and I&#8217;m lucky to be working with a code-base that many consider to be an example in programming practices (by and large, but not entirely). I&#8217;m also working with everyone else on improving bfiles, an extension meant to improve the way Mercurial deals with big/binary files, and my first order of business is supporting HTTP uploads.