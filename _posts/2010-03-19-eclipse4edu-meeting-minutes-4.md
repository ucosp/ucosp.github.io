---
id: 2661
title: Eclipse4Edu Meeting Minutes
date: 2010-03-19T18:47:07+00:00
author: Brenda Sadoway
layout: post
guid: http://ucosp.wordpress.com/?p=2661
permalink: /2009-2010/eclipse4edu/2010/03/eclipse4edu-meeting-minutes-4/
categories:
  - Eclipse4Edu
  - Status
---
We had a brief meeting today and here is the summary.

Present: Brenda, Cory

Absent: Miles

**Drag and Drop**

&#8211;          Cory is still plugging away at implementing this, as it is not a small task.  If anyone is interested in looking at it and providing feedback, it would be beneficial.

&#8211;          He is also wondering if anyone has priorities or features in mind in regards to drag and drop.

**Class Wizard**

&#8211;          Brenda intends to refactor her patch for fixing the package dropdown menu to separate UI from the model.

&#8211;          Making a package constructor is something to look into.  This could potentially lead to moving class lookup into the class constructor and package lookup into the package constructor.  Possibly by making static methods such as findClasses(project, package).

**Simplify Menus**

&#8211;          Miles is working on this and has posted patches and comments marking his progress on Bug 299848.