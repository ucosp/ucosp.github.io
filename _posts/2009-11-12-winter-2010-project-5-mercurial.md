---
id: 1275
title: 'Winter 2010 Project #5: Mercurial'
date: 2009-11-12T21:03:16+00:00
author: Greg Wilson
layout: post
guid: http://ucosp.wordpress.com/?p=1275
permalink: /2009-2010/mercurial/2009/11/winter-2010-project-5-mercurial/
categories:
  - Mercurial
  - Proposals
tags:
  - Winter 2010
---
The [Mercurial](http://mercurial.selenic.com/) distributed version control system is used by thousands of developers. NetBeans, OpenJDK, OpenOffice, and Python itself are just a few of the projects that have adopted Mercurial as their version control system. But as much as Mercurial has been making incredible inroads in the open-source community, it has some key deficiencies that make it a poor choice for real-life commercial development.

Here at [Fog Creek Software,](http://fogcreek.com/) we&#8217;re about to release a brand-new source control management system called Kiln that&#8217;s based on Mercurial. As part of that project, we want to fix the problems in Mercurial that currently prevent commercial development shops from adopting it with the same enthusiasm as their open-source counterparts.

That&#8217;s where you come in. In UCOSP, you will focus on improving Mercurial&#8217;s performance and user. More specifically, you&#8217;ll:

  * Improve the handling of binary files
  * Improve support for very large repositories
  * Add support for secure password management
  * Improve end-user feedback during lengthy network operations
  * Improve history viewing tools

Once you&#8217;ve implemented these improvements, we&#8217;ll be sending them to the Mercurial project, which has a highly supportive developer community and a predictable release schedule. So you&#8217;ll have a really high chance of seeing your code in production soon after the project ends.

Mercurial is written in high-level Python and low-level C, and has relatively complex on-disk formats and network protocols. Because we&#8217;ll be touching most of the stack, you&#8217;ll feel most comfortable if your past experience runs the gamut from high- to low-level work.

Mentor: Benjamin Pollack ([Fog Creek Software](http://www.fogcreek.com))