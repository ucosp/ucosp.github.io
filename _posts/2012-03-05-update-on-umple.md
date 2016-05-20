---
id: 2862
title: Update on Umple
date: 2012-03-05T17:14:08+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2862
permalink: /winter-2012/2012/03/update-on-umple/
categories:
  - Winter 2012
---
Jordan Johns writes:

The second month of the [UCOSP Winter 2012 Umple project](https://code.google.com/p/umple/wiki/UCOSP) has been quite a good experience for many involved. Everything from bug fixes, compiler enhancements and new features have been accomplished thus far.

It has been a really good experience. I&#8217;ll start off by mentioning what has been going on with the others students.

To begin with we&#8217;ve had James who has been diligent in working on enhancing the capabilities of the compiler, by enabling additional command line options. A particularly good use of the recent enhancements in this aspect are that you can specify the output language of the generated code on the command line; his objective is to enable the Umple compiler to compile the Java, so any Java error messages appear as Umple error messages.

Sonya has had a breakthrough with enabling a rather useful feature to Umple: class-evel immutability. With this new feature, those who wish to use Umple to build systems in, lets say, Java can create immutable classes with ease.

Another good addition, that is in progress at the current moment in time, is SQL code generation. Adam has been making some headway in this regard and soon we will have the ability to create usable SQL code from the Umple code we write.

With respect to primary enhancements this is where we&#8217;re at currently, however bug fixes have seen quite a bit of progress. Luna has been working on fixing deletion of 1-* associations at the many end in PHP and Ruby; this currently fails. Another fix being worked on by Song Bae is to fix a rather interesting problem in UmpleOnline where class names do not correspond to association names when the former is changed. 

My tasks have been fixing issues mainly associated with the compiler and providing maintenance in relation to codebase documentation. I&#8217;ve made a decent amount of progress on this I think.

To start off with we&#8217;ve had a issue where you could write comments in your Umple code but when you generate code from it, such as Java code, not all the comments would appear. Although the generated code is not intended to be read by developers (e.g. it ought to be treated in the same manner as bytecode or machine code), there are two reasons why comments nonetheless need to appear: First is that tools such as JavaDoc or Eclipse ToolTips generate API documentation from the comments; second an objective of Umple is to demonstrate what good-quality generated code would look like. The lack of comments meant, for example, that those developing Umple itself couldn&#8217;t make good use of any internal documentation.

The initial learning curve a while back was essentially this, figure out how the codebase is working and look into fixing this problem. As it turned out this meant that I had to get really familiar with the compiler parser to ensure that comments follow out to the generated output. After learning the parser and getting acquainted with a few different areas of the project I was able to fix the problem, which now allows comments of consistent format to appear in generated code. This is quite good, because now internal documentation problems can be solved which is what I&#8217;m currently trying to do.

I really like the codebase and wish those who follow to have a solid base to work off of, and knowing the learning curve associated with a very large codebase I want to ensure they have good documentation to assist in that regard.

So everything from compiler enhancements and new features to bug fixes and internal documentation (maintenance), I would say good progress is being made. I personally really like the Umple project, the mentors are extremely knowledgeable and always willing to assist when there is a problem. The project itself has a good purpose and I think others should try it out and use it. It really does save time to create a system really quickly since you essentially write a little bit of Umple code and get a lot of consistent workable generated code in almost any language from Java, C++, Ruby or PHP. I definitely see Umple as a great project to work on, thus far I have enjoyed it, and I hope to see how it turns out later on.