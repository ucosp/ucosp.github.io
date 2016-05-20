---
id: 2269
title: 'Status Reports: Feb 8, 2010'
date: 2010-02-10T13:17:08+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2269
permalink: /2009-2010/eclipse4edu/2010/02/status-reports-feb-8-2010/
categories:
  - Eclipse4Edu
  - Status
---
## **Brenda**

### Status

  * Submitted a patch for Bug 299965 so that the default package and src folder are hidden, but explicitly made packages and other source folders are not (for the sake of comparing different approaches to this problem).
  * Submitted a patch for Bug 300388 to rename the Scheme interpreter extension point and schema. 

### Next Steps

  * Look into the Scheme perspective more and some of the bugs that have been opened in regards to that (for example, Bugs 299866, 299867 and 299868).

### Roadblocks

<ul type="disc">
  <li>
    None
  </li>
</ul>

* * *

## **Cory**

### Status

  * Put forth a list of ideas / suggestions on areas to improve the usability of Java Lite and emailed that out to the mailing list.
  * Posted some results of my research towards simplifying toolbars / menus (Bug 299848).
  * Added a new patch for Bug 299689 (fixed go to workbench link from start screen).
  * Added 2 new bugs and posted a patch to address them. (Bug 302052 &#8211; Refactoring out LiteLaunchShortcutsAction, and Bug 302054 &#8211; renaming JavaLiteProjectWizard to match other source files, the posted patch also address an NPE). 

### Next Steps

  * Continuing to work on small bugs. Might look into Bug 299878 (dragging files) or Bug 299873 / 875 (deleting items). 
  * Will be bringing up some questions regarding the future of the java lite package explorer, and if these bugs are worth fixing given the current state of the class. 

### Roadblocks

<ul type="disc">
  <li>
    Other classes; I&#8217;ve been extremely busy the previous week, and this week isn&#8217;t looking very good either. Also, reading week begins next week, and midterms are shortly thereafter..
  </li>
</ul>

* * *

## **Miles**

### Status

  * Working on the templates for class creation to distinguish between “programs” (classes with main methods) and “classes” (object oriented programming units).
  * Tried to figure out how to get a Template evaluated and put the generated code back into the CompilationUnit. Not sure this is going to work or be worth the effort. I thought this might be a more elegant way to deal with the information already stored in the CompilationUnit like the class name and the package name.
  * May need to just generate the text all at once in the action or wizard and then send the text to the class constructor.

### Next Steps

  * Continue working on initial code generation. Hope to get a couple of ideas developed.

### Roadblocks

<ul type="disc">
  <li>
    Trying to figure out how to avoid internal JDT code is difficult.
  </li>
  <li>
    I suspect this is going to be a major roadblock for this project. Reinventing the wheel for each thing we want to do is not going to be fun.
  </li>
</ul>

* * *