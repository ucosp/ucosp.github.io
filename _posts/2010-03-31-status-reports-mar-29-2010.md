---
id: 2707
title: 'Status Reports: Mar 29, 2010'
date: 2010-03-31T15:04:52+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2707
permalink: /2009-2010/eclipse4edu/2010/03/status-reports-mar-29-2010/
categories:
  - Eclipse4Edu
  - Status
---
Brenda</strong></h2> 

### Status

  * Looked further into Bug 303420: Simplify the user experience when renaming a type from the pop-up menu. This may not actually be a task I can accomplish before the code freeze, taking into account the other things I had also intended to finish before then.

### Final Steps

  * Look into Bug 303420: Simplify the user experience when renaming a type from the pop-up menu.
  * Go back to Bug 299342: "New Java Package" option should automatically create a Java Project, to use the NewJavaProjectConstructor to create the default project.
  * Address Bug 303427: Can&#8217;t specify a source folder in the Package Wizard.
  * Complete final report.

### Roadblocks

<ul type="disc">
  <li>
    Last week involved several major deadlines for other courses, but I can now focus this week on finishing up my ongoing goals for Eclipse..
  </li>
</ul>

* * *

## **Cory**

### Status

  * Added some additional comments to Bug 301327 (Creating a src folder when creating new Java project &#8211; This bug may not be applicable anymore) and to Bug 302362 (Support for java applets &#8211; This bug may also be obsolete now).
  * Overall, I did not have a productive week with regards to IDE4EDU. Still waiting on feedback from Wayne, and at least 50%+ of our bugs require some form of feedback, committing, closing, or additional information. So, I took this opportunity to work on my many other projects and their fast approaching deadlines, with the hope that when Wayne gets back I will be able to dedicate more time towards IDE4EDU. 

### Final Steps

  * Of the bugs left that aren&#8217;t in 1 of the categories above, I think I might take stab at Bug 302360 (importing projects into javalite) or Bug 303584 (Linking javalite explorer with editor). In both cases, there is existing JDT functionality that we want to emulate, so they sound feasible given our remaining week before the code freeze.
  * Unless of course we get feedback from Wayne, in which case I will attempt to address those potential issues, etc. 

### Roadblocks

<ul type="disc">
  <li>
    (I know its a broken record&#8230; but) Other classes.
  </li>
  <li>
    Feedback would be appreciated on pending patches. (We are here to help! Let us help!)
  </li>
</ul>

* * *

## **Miles**

### Status

  * Worked on simplifying the menus using the activities extension.
  * Managed to hide all but 2 or 3 things that I wanted hidden.
      
    &#8211; Simplified the toolbar significantly. 
      
    &#8211; Really happy with how this turned out. Makes Eclipse much less intimidating.

### Final Steps

  * Simplify the menus and toolbar to the list of items I suggested in bug 299848.

### Roadblocks

<ul type="disc">
  <li>
    Nothing major. Everything is working out pretty well on this bug. I&#8217;d like to control the order of the toolbar buttons but I can&#8217;t figure out<br /> how to do that yet. Also, I&#8217;d like a couple of the menus to go away when they don&#8217;t have any items in them like the Run menu.
  </li>
  <li>
    I&#8217;d love to hide the Navigation menu but it seems to be hardwired to the Workbench or something. I think we&#8217;d need to create an RCP app to<br /> completely get rid of it.
  </li>
  <li>
    We need to create a better Run and Debug button but that is too big a job for the time we have left on this project. I&#8217;ll add another bug for this.
  </li>
</ul>