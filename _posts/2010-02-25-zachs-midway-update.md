---
id: 2390
title: 'Zach&#039;s Midway Update'
date: 2010-02-25T22:10:59+00:00
author: zgchurch
layout: post
guid: http://ucosp.wordpress.com/2010/02/25/zachs-midway-update/
permalink: /2009-2010/uncategorized/2010/02/zachs-midway-update/
categories:
  - Uncategorized
---
I&#8217;m definitely feeling better about working on projects with \_huge\_ codebases like Thunderbird. I&#8217;m currently working on a patch to add a &#8220;Reopen last tab&#8221; button to Thunderbird. I&#8217;m finally feeling like I know my way around Thunderbird&#8217;s tab management code. I submitted a patch a couple weeks ago and got some feedback, and I&#8217;ve done most of what the patch suggested. The only thing left to do before I submit my patch again is to figure out why the UI tests sometimes pass and sometimes fail on my computer (even without my patch applied!) After I get that figured out, I need to write a few more UI tests. After that I&#8217;ll be ready to submit my patch again.

My next patch will to create a menu of recently closed tabs, so the user can select from several tabs that they&#8217;ve just closed, similar to in Firefox.