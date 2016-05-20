---
id: 2465
title: 'Kefu Zhao &#8212; Midterm Update'
date: 2010-03-01T00:56:03+00:00
author: fishz48
layout: post
guid: http://ucosp.wordpress.com/?p=2465
permalink: /2009-2010/uncategorized/2010/03/kefu-zhao-midterm-update/
categories:
  - Uncategorized
---
**My Goal and Expectation**

My work at Thunderbird is mainly to fix a bug regarding to the “Reply To List” feature. By working on this bug, I am expecting to get myself further exposed to real industrialized products based on my computing science knowledge gained from previous school and work experience.

**What I have done so far and What have I learned**

First of all, I have to say that my ability to analyze problems is greatly enhanced through working on Thunderbird, which is a complicated software comprising million lines of code. Before I start coding, I have to fully understand what the bug is and decide the scope in which the bug is located. Also, I need to know how relative code works and see why it’s going wrong. Then, I can propose an enhancement suggestion and start adding my code fix to existing structure. During this process, I need to talk to people through IRC and try to find materials to solve my problems. All in all, this is a really valuable experience.

Secondly, my ability to debug is improved. Before I work on Thunderbird, I used to debug while I am programming simultaneously. There are two reasons for me to do this:

1)      There are convenient debugging tools such as eclipse and Visual Studio.

2)      The compile time is relatively fast (almost instantly).

Given these two reasons, I wasn’t used to considering the problem thoroughly before I start debugging. However, things are different in Thunderbird because on one hand, _Venkman (JavaScript debugger for Thunderbird)_ _is not totally reliable at all the times. On the other hand, it usually takes a relatively long time to compile my changes. As a result, I need to thoroughly consider my problem to every detail before I start compiling. Without any doubt, this is an absolute good habit for programmer._

_Last but not least, I learned some new technologies and my programming ability is greatly enhanced. Thunderbird uses XPCOM that is_ a cross platform component object model. It brings multiple languages support as well as a set of unified API for us to call. Despite the lack of documentations, we can still get well use of these API by viewing relative idl files.

**What’s Next**

In the rest of this semester, I will finish up my patch for the bug and write some test for it. Hopefully I can successfully deliver my patch to the products.

Good luck to all of us,

Kefu