---
id: 2414
title: Eclipse4Edu Meeting Minutes
date: 2010-02-26T22:05:11+00:00
author: Brenda Sadoway
layout: post
guid: http://ucosp.wordpress.com/?p=2414
permalink: /2009-2010/eclipse4edu/2010/02/eclipse4edu-meeting-minutes-3/
categories:
  - Eclipse4Edu
  - Status
---
We had a brief meeting today; here is what we discussed.

**Present:** Miles, Cory and Brenda

**Absent:** No one

 ****

**Naming**

&#8211;          Educlipse (or EduEclipse) is short, concise and demonstrates what it is – a version of Eclipse meant for education.

&#8211;          Eclipse IDE for Education fits well with the naming schemes for other Eclipse products.

&#8211;          The consensus between us still seems to be Educlipse or EduEclipse, however.

 ****

**Templates**

&#8211;          Discussed opening an extension point for the templates; we shouldn’t need more than 2-4 templates ourselves.

&#8211;          There could be  a problem if we want to allow others to add and manage templates, but it doesn’t seem to be a high priority at the moment.

**“New Java Program”**

&#8211;          Seems like a good idea to simplify the process initially for users that may not even understand the concept of a class within a project yet.

&#8211;          Possibly greyed out text in the project explorer: “Create a new project or program to get started”.

&#8211;          The Scheme perspective that hasn’t been committed (see Bug 293093) handles help/tutorials well, as far as introducing the user to what they can do and how they can do it.  Something similar to this in Java Lite might be worthwhile.  A “Start Coding in Java” link on the intro page would open Java Lite, and the user would immediately have access to the hints/tips in the help view so they can get started.

**Hiding source folders and default packages**

&#8211;          Cory submitted a patch that should fix the problems with the view not refreshing and new classes not being selected upon creation.

&#8211;          There is still the issue of having two packages with the same name in different source folders appearing side by side in the Java Lite project explorer.  There are different ways we could handle this, but it’s not a high priority to fix right now.