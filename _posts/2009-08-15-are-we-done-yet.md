---
id: 82
title: Are We Done Yet?
date: 2009-08-15T11:17:40+00:00
author: Greg Wilson
layout: post
guid: http://ucosp.wordpress.com/?p=82
permalink: /2009-2010/education/2009/08/are-we-done-yet/
categories:
  - Education
---
One of the questions programmers often ask (and are often asked) is, &#8220;Are we done yet?&#8221; It&#8217;s often hard to know: unlike spaghetti, you can&#8217;t just throw software against the wall to see if it sticks. &#8220;When we run out of time&#8221; and &#8220;when we run out of money&#8221; are common answers in the real world, but there are better ways, and [this page](http://people.mozilla.com/~mnandigama/codecoverage_html/) shows one of them. Each row represents a module in Firefox; the numbers show what percentage of the lines and functions in that module are exercised by tests. The goal definitely isn&#8217;t to get 100% coverage of every module&#8212;that&#8217;s usually impossible, almost always uneconomic, and still doesn&#8217;t guarantee that the program will work [1]. It&#8217;s also misleading to think that high coverage automatically means high reliability [2]. What it _does_ do is draw attention to places where we just don&#8217;t know what the quality of the code is. As a bonus, if coverage from past test runs is stored somewhere, tables like these can tell us if the percentage of tested code in a module has suddenly gone down, i.e., if someone has added several hundred lines of new functionality without adding corresponding tests.

So why aren&#8217;t coverage stats like these taught in first year programming courses and expected afterward? Setting up a server to run tests automatically every hour and refresh a page like the example is a bit of work, but IDEs like Eclipse can equally well measure and report coverage on the developer&#8217;s desktop.  As with many other working practices, I think there are two reasons:

  1. Inertia: we didn&#8217;t do it twenty years ago, so today&#8217;s teachers don&#8217;t think it&#8217;s a must-have, so they don&#8217;t teach it to today&#8217;s students, and around and around we go.
  2. Time pressure: every undergraduate curriculum (not just that of computer science) is already overcrowded. As simple as this idea is, adding it would mean less time for something else, and no one can agree on what &#8220;something else&#8221; to take out.

[1] See [Wikipedia&#8217;s discussion of code coverage and path coverage](http://en.wikipedia.org/wiki/Code_coverage).

[2] Particularly for concurrent code&#8212;even if every individual path works correctly, the interactions between multiple processes or threads can cause race conditions, deadlocks, and partial failures.