---
id: 2654
title: 'Status Reports: Mar 15, 2010'
date: 2010-03-17T18:12:29+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2654
permalink: /2009-2010/eclipse4edu/2010/03/status-reports-mar-15-2010/
categories:
  - Eclipse4Edu
  - Status
---
## **Brenda**

### Status

  * Reworked the patch for Bug 303426 to fix the problem Wayne noted.
  * I found the solution to Bug 303581 and included it in this patch as the code greatly overlapped and the problems were related. Made note of this in Bug 303581.
  * Started investigating into Bug 303420 (Simplify the user experience when renaming a type from the pop-up menu) to see how this should be done. I have the main outline coded, but I&#8217;m still figuring out how to pull in the refactoring functionality to use in conjunction with this code.

### Final Steps

  * Finish what I started this week on the class constructor (TODOs and Bug 301326: NewJavaClassConstructor#construct() needs to be more robust).
  * Look into Bug 303420: Simplify the user experience when renaming a type from the pop-up menu.
  * Go back to Bug 299342: "New Java Package" option should automatically create a Java Project, to use the NewJavaProjectConstructor to create the default project.
  * Address Bug 303427: Can&#8217;t specify a source folder in the Package Wizard.
  * Complete final report.

### Roadblocks

<ul type="disc">
  <li>
    Last week of midterms.
  </li>
</ul>

* * *

## **Cory**

### Status

  * Still quite busy with plenty of other schoolwork. Approaching end of term, and its always hectic.
  * Did get some time last weekend to do some more work on the drag and drop implementation. (See Bug 299878 for more info). 
  * I ended up refactoring some code, and made the drag and drop listener implementations a little less "exotic". 
  * Will be following this update with a new patch to the bug. 

### Next Steps

  * Due to code halt within the next 2 weeks, I figure it might be best for me to keep working on the drag and drop implementation.
  * There is still a couple "major" issues to sort out, and I will try and fix those up. Namely, providing the ability to detect if a name conflict exists before attempting the move, and then provide the user the ability to change the file name. 
  * Small stuff like &#8211; I have a good 6-8 TODOs to fix in the code, and I&#8217;m sure wayne will want to add his 2 cents in as well.
  * It would be nice if we got some feedback on all pending patches, so we can make sure they get finished / committed before the end of the course. 
  * Complete final report.

### Roadblocks

<ul type="disc">
  <li>
    Other courses.
  </li>
</ul>

* * *

## **Miles**

### Status

  * Worked on simplifying the menus using the activities extension. 
  * This seems to work quite well but complete control over the menus is still elusive.
  * There are a bunch of things I can remove and a few things that stubbornly won’t go away.

### Final Steps

  * Figuring out how to simplify the menus. If this goes smoothly I will try to apply the lessons learned to simplifying the tool bars.
  * Complete final report.

### Roadblocks

<ul type="disc">
  <li>
    Just difficulty figuring out how to get complete control over the UI.
  </li>
</ul>