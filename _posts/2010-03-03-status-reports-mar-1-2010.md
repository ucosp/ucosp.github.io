---
id: 2595
title: 'Status Reports: Mar 1, 2010'
date: 2010-03-03T14:14:33+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2595
permalink: /2009-2010/eclipse4edu/2010/03/status-reports-mar-1-2010/
categories:
  - Eclipse4Edu
  - Status
---
## **Brenda**

### Status

  * Worked with Cory on fixing the patch I submitted for Bug 299965 (updating the view when a class is made in the default package of a project with a source folder). He made the fix and submitted the patch.
  * Submitted a patch for Bug 303426 (Class Creation Wizard lists projects in the package selection menu). It fixes the main problem, but is not complete yet. 

### Next Steps

  * Implement the second step for Bug 303426 so that the list of packages updates when the currently chosen project is changed.
  * Look into highlighting the currently selected item from the dropdown list.

### Roadblocks

<ul type="disc">
  <li>
    None.
  </li>
</ul>

* * *

## **Cory**

### Status

  * Assisted Brenda on hiding package references (Bug 299965). I think we figured out the refresh issue, and I posted a new patch fixing that.
  * Started work on the drag and drop feature (Bug 299878). Submitted a first-pass patch towards this feature.
  * I dedicated a fair bit of hours to eclipse this past week as I had a break in my other classes; I&#8217;m expecting my next week or so will be dedicated to those classes instead &#8211; as usual I get plenty of new assignments at the last minute. 

### Next Steps

  * Continue work on drag and drop.
  * Look into small things as they arise. 

### Roadblocks

<ul type="disc">
  <li>
    Other classes
  </li>
</ul>

* * *

## **Miles**

### Status

  * Refactored sections of the new Class creation wizards and constructors. 
  * Moved more of the customizability of the wizards and constructor to the templates so that the templates along with a template specific action really drive all of the differences between templates in the rest of the classes.

### Next Steps

  * Mostly the same as my last report.
  * Add further functionality to the Class creation constructor and wizards specifically relating to packages.
  * Make is so the Package field in the Class creation wizard is only displayed if there are packages created in the workspace.
  * I would really like to start spending some time on figuring out how to simplify the menus and toolbars. This is such a big problem with the plug-in that it would be nice to get this fixed by the end of the semester.

### Roadblocks

<ul type="disc">
  <li>
    No real roadblocks.
  </li>
  <li>
    I guess I would love to get some higher level feedback on the refactoring that has been done to the new Class constructor and wizards. Thoughts about the way things are fitting together, other possible designs, as well as what kinds of issues to be aware of when writing this kind of code would be educational.
  </li>
</ul>

* * *