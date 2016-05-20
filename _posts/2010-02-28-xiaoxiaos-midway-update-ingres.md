---
id: 2459
title: 'Xiaoxiao&#039;s Midway Update-Ingres'
date: 2010-02-28T21:26:29+00:00
author: George
layout: post
guid: http://ucosp.wordpress.com/?p=2459
permalink: /2009-2010/ingres/2010/02/xiaoxiaos-midway-update-ingres/
categories:
  - Ingres
  - Status
---
My overall progress is a bit slower than I expected, because environment setup took me too long in early February. But I have started implementing actual code and current progress seems good.

The main difficulty I have had so far is setting up development and testing environment. A large scale open source project such as geotools requires me to install and configure a lot of programs before development starts. Therefore, this setup progress is time-consuming and requires attention to detail.  I set one argument in a single program&#8217;s configuration to a wrong value, and the whole project wouldn&#8217;t build. This mistake wasn&#8217;t discovered until after I spend 5 days double checking all settings and with Lim&#8217;s help. Moreover, a Ubuntu crash forced me to reinstall the system and to started all over again. However, I find this (rather painful) process valuable and rewarding, since this is the first time I need to do so many configurations at the same time(linux, java, eclipse, mvn, geotool, geoserver, openvpn) to make software work.

The reading overhead is also much more than the actually development. I have to spend at least 3 hours per week to read online documentations, mailing lists, and book.

But the overhead in setting up environment and reading greatly helps us to understand what we need to write. Writing code is really the last and easiest thing to do if you can understand the problem to solve.