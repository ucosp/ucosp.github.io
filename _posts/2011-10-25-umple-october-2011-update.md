---
id: 2844
title: UMPLE October 2011 Update
date: 2011-10-25T17:49:46+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2844
permalink: /2009-2010/uncategorized/2011/10/umple-october-2011-update/
categories:
  - Fall 2011
  - Uncategorized
tags:
  - Fall 2011
  - Status Update
---
The Umple project is advancing rapidly this semester with three UCOSP students making major contributions in parallel with other contributors.

UCOSP students are have tackled some smaller features and bugs, and are now working on a couple of long-standing major issues: Generating comprehensive and useful error messages, and getting rid of certain syntax oddities.

Dr. Lethbridge, the project mentor, just posted a [blog post](http://tims-ideas.blogspot.com/2011/10/umple-status-and-recent-progress.html "blog post") that covers the recent work in technical detail:

We asked each of the three UCOSP students to highlight what they have been learning and doing, what they have liked about the project so far, and what improvements they think they would like to see to how Umple is developed or the how UCOSP program is run.

**From Joshua Horacsek:**

Basically, I&#8217;ve been working on making Umple more user-friendly. I&#8217;ve been reworking the way Umple handles lexical and semantic errors, hopefully making it more robust, and ultimately more useable.

My favourite part of Umple isn&#8217;t necessarily what the project aims to accomplish, but rather how the different components of Umple are built, what they&#8217;re built with, and how they interact. That&#8217;s not to say the idea of a model based language isn&#8217;t interesting, it&#8217;s just that Umple&#8217;s a fairly large project, and it&#8217;s pretty fun to navigate.

I&#8217;ve learned how to look at a fairly large project with multiple different components, and break it down into components that I understand. I&#8217;ve also learned the benefit of test driven development, and the headaches and time it saves.

As of right now, I have two primary goals. The first is to get Umple to a point where it produces concise error feedback for a wide variety of input. The second goal is tied to code generation from an Umple model. Currently, Umple can generate code for various languages such as Java, PHP and Ruby. If I have time I&#8217;d like to extend it to generate SQL models, and if not, at least there&#8217;ll be some partial code for a future UCOSP project.

From my perspective, I can&#8217;t really see what either UCOSP or Umple could be doing better for UCOSP students.

**From Alvina Lee:**

I am working on a feature which allows umple to generate comments before classes. I made patches for issues regarding lazy keywords for attributes in generating singleton classes as well as automatically changing associations from 1 to 0..1 (issue 26).

I like that I get to learn new things and make use of computer science related stuff I&#8217;ve used before.

What I am learning:

• Using JUnit on larger projects
  
• Learning to work with other people who do not live in the same area on the same project
  
• Learning to use new technology that I am not familiar with
  
• Learning about UML

By the end of this term, I will have some involvement with error parsing and have commenting for attributes and other objects implemented.

What the project could be doing better: Umple has included some video tutorials. While I appreciate the fact that they are offering help in setting up the developing environment, I do not like video tutorials because I have to wait to download them, and I dislike the format because it is harder to skip around to relevant sections if I am already familiar with what is being explained in some parts of the tutorial.

**From Joel Hobson:**

My name is Joel Hobson, and this is my first blog post for the UCOSP project and Umple. I&#8217;m currently working on two main tasks for Umple &#8211; First, I&#8217;m working on adding a debug mode for developers that shows which JET templates generate specific code, in order to make it easier to add new languages to Umple. My other main task is fixing the various bugs regarding whitespace. Umple is currently finicky about whitespace, and code that programmers would expect to be valid, such as class X { attributeName=&#8221;&#8221;; } causes problems.

I&#8217;ve never had the opportunity to work on a large software project before, and I&#8217;ve greatly enjoyed the experience. Umple is a very interesting project, and I feel it could be extremely useful for large software projects when it becomes a little more mature.

Working on Umple, I&#8217;ve learned a great deal about test-driven development. I had a vague understanding of the concept before, but now that I&#8217;ve actually used it I can see just how useful it is. I&#8217;ve also gained experience working with Apache Ant and Subversion, and have a much better idea of how contribution to open source projects works. The biggest challenge so far was getting it to build correctly on my system. Even now, I have some difficulty with errors in the build process, but overall things are going fairly smoothly.

My goals for the project include finishing the debug mode and fixing the whitespace bugs, as well as writing Umple extensions for various text editors and fixing random bugs, time permitting.