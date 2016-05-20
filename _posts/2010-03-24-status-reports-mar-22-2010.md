---
id: 2677
title: 'Status Reports: Mar 22, 2010'
date: 2010-03-24T13:28:58+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2677
permalink: /2009-2010/eclipse4edu/2010/03/status-reports-mar-22-2010/
categories:
  - Eclipse4Edu
  - Status
---
## **Brenda**

### Status

  * Submitted a patch to Bug 301326 to handle the possibility of multiple source folders when creating a new class using the constructor.
  * Reported Bug 306651 and submitted a patch for it that creates a package constructor like those for projects and classes, including tests. It also includes a rework of the Package Creation Wizard to use the constructor, along the lines of the project and class wizards.

### Final Steps

  * Look into Bug 303420: Simplify the user experience when renaming a type from the pop-up menu.
  * Go back to Bug 299342: "New Java Package" option should automatically create a Java Project, to use the NewJavaProjectConstructor to create the default project.
  * Address Bug 303427: Can&#8217;t specify a source folder in the Package Wizard.
  * Complete final report.

### Roadblocks

<ul type="disc">
  <li>
    None.
  </li>
</ul>

* * *

## **Cory**

### Status

  * I continued development on the DND implementation as mentioned last week.
  * I completed some more refactoring and added in some rough name conflict / resolution code. There are still bugs to work out unfortunately.
  * I also investigated into just using existing JDT internal DND implementations, and posted my comments towards that on the current DND bug as well. 

### Next Steps

  * Possibly more work on DND pending feedback on my latest comments towards the DND bug.
  * Otherwise, I will try and find something thats doable within the next week or so, and work on that instead.
  * Complete final report.

### Roadblocks

<ul type="disc">
  <li>
    Other courses.
  </li>
  <li>
    Waiting on input from Wayne on pending drag and drop changes.
  </li>
</ul>

* * *

## **Miles**

### Status

  * Worked on simplifying the menus using the activities extension.
  * Made a couple of breakthroughs on how to figure out what id to use to hide items.

### Final Steps

  * Simplify the menus to the list of items I suggested in bug 299848.
  * If this goes smoothly I will try to apply the lessons learned to simplifying the tool bars.
  * Complete final report.

### Roadblocks

<ul type="disc">
  <li>
    There are still a few items that won&#8217;t go away as they seem to be &#8216;special&#8217; to the workbench or something. For example &#8216;File/Revert&#8217; and<br /> &#8216;Edit/Delete&#8217; are 2 of them. But there aren&#8217;t that many of them and they aren&#8217;t too confusing to the user.
  </li>
</ul>