---
id: 2171
title: 'Status Reports: Jan 25, 2010'
date: 2010-01-27T16:17:05+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2171
permalink: /2009-2010/eclipse4edu/2010/01/status-reports-jan-25-2010/
categories:
  - Eclipse4Edu
  - Status
---
## **Brenda**

### Status

  * Worked on Bug 299965 to hide packages from the user and posted a patch for the bug.
  * An outstanding issue with this however is that if a project is made outside of Java Lite, the src folder and any packages within it are visible (that is, the patch works for projects made through the Java Lite project wizard only).

### Next Steps

  * Work on the issue mentioned above so that projects made outside the Lite perspective will also hide packages (and the src folder). 

### Roadblocks

<ul type="disc">
  <li>
    None
  </li>
</ul>

* * *

## **Cory**

### Status

  * Been trying to learn how to hide toolbars / menus. 
  * Looked at the links you sent miles (and many other links too), but I&#8217;ve been unsuccessful in getting the activity extension point to work on different plugin contributions.
  * Been investigating if it would be better suited as part of an RCP app tailored to our purposes. I setup an rcp app for myself and I think it will be doable going this route as we can override the menu managers to not accept other plugin contributions. This is still in theory though&#8230;
  * Updated the given bug patch to add line numbers to the editor by default. And posted another patch to fix a couple more warnings. 

### Next Steps

  * Continuing to try and remove / block unwanted toolbars and menu items, most likely from an RCP app instead of inside our already created plugins. 

### Roadblocks

<ul type="disc">
  <li>
    Eclipse framework &#8211; The activity extension point seems to take additional, unmentioned magic.. Wish they had better tutorials / examples of how things work with one another.
  </li>
</ul>

* * *

## **Miles**

### Status

  * On the weekend I mainly worked on creating a Java class constructor class as per Wayne’s bug for this. 
  * Currently this is done in a wizard called NewTypeWizardPage and all of the class creation code is intermingled with the wizard code. 
  * I also trried to wrap the NewTypeWizardPage to see if there was a way to leverage the 2500+ lines of code in that class. Wayne and I discussed it and the first option appears to be the best way forward.

### Next Steps

  * I am going to get the basic version cleaned up, write some more tests for it and try to get a simple class construction wizard up and running.
  * I am going to continue working on this constructor class and make it a bit more full featured: 
      * oAllow extending superclasses, implementing interfaces, initial templates, etc.
  * I would like to also do some brainstorming of how we can make the new class wizard more useful to students.

### Roadblocks

<ul type="disc">
  <li>
    No major roadblocks at this point. I think I need to figure out a bunch more stuff about the JDT Java Model.
  </li>
</ul>

* * *