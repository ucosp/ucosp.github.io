---
id: 2116
title: 'Status Reports: Jan 18, 2010'
date: 2010-01-20T15:40:21+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2116
permalink: /2009-2010/eclipse4edu/2010/01/status-reports-jan-18-2010/
categories:
  - Eclipse4Edu
  - Status
---
Brenda</strong></h2> 

### Status

  * Attended the Code Sprint
  * Spent a lot of time looking through the code, getting an idea for the framework.
  * Reported several bugs for the Java Lite perspective.
  * Tested the patch for Bug 244645 (making a new class in an empty workspace). I agree with it and also posted a new bug (299342) with a patch that does the equivalent for making a new package. However, after the code sprint, we decided that packages should be done away with overall (that is, hidden). 

### Next Steps

  * Submitting a bug for hiding the concept of packages from the student, and working on it. 

### Roadblocks

<ul type="disc">
  <li>
    None
  </li>
</ul>

* * *

## **Cory**

### Status

  * Not much work done before code sprint &#8211; mainly attempting to setup environment, and emailed out some first impressions of the current state of the program. 
      * Code sprint:
          
        &#8211; Attempted to apply as many patches as possible, and test how they work.
          
        &#8211; Used both scheme and java lite for some basic coding &#8211; attempted to use a "1st year / 1st time coding" perspective while using the eclipse plugins.
          
        &#8211; Also looked into some competing plugins &#8211; namely pneumbra and how that tied into the eclipse framework.
          
        &#8211; Added a bunch of new bugs to bugzilla (8 or so) that I noticed with scheme and the java lite views.
          
        &#8211; Did a fair bit of work trying to learn the framework.
        
        &#8211; Added a patch to https://bugs.eclipse.org/bugs/show_bug.cgi?id=288854 to address about half the warnings (includes all of the arraylist ones though). 
         
        &#8211; Also posted some additional comments wrt. that bug / patch.
    
    
        

### Next Steps

  * To put it bluntly, the eclipse UI needs a lot of work to be beginner programmer friendly. I&#8217;m going to try and work on reducing UI clutter, unneeded UI elements (including menus, toolbars, context menus, etc) for the java lite perspective.
  * I think customizing the RCP app will take us a step in this direction. 

### Roadblocks

<ul type="disc">
  <li>
    The Repository. Having to constantly update the project set seems to be a hassle&#8230; Are there any of important files that we may need / should be aware of before getting into the thick of development?
  </li>
</ul>

* * *

## **Miles**

### Status

  * On the weekend I mainly worked on figuring out how to simplify the menus. We made some progress by creating a perspective listener and removing all of the action sets from it.
  * I managed to learn enough to actually fix a bug. When a project is created automagically on class creation in an empty workspace, src and bin folders were created. I found out how to turn this switch off so that the src and bin folders are not created.
  * I figured out that when you create a patch you need to make sure you don’t have any other patches installed for other unrelated bugs so your patch doesn’t incorporate those changes.

### Next Steps

  * I would like to work on the menu and toolbar simplification but Cory has claimed that. I’ll let him work on that and chip in later if he needs help.
  * I think I am going to take a look at one of 2 things: 
      * A Java Lite debugging perspective that illuminates concepts like scope, static space, the stack and the heap
      * The templates for class creation to distinguish between “programs” (classes with main methods) and “classes” (object oriented programming units)
    
    
        

### Roadblocks

<ul type="disc">
  <li>
    There are some menu items and tool bar items that do not appear to be ActionSets. I can’t figure out what they are and how to get rid of them.
  </li>
  <li>
    Figure out how to get access to the debugging information and how to create and modify a Java Lite Debug perspective.
  </li>
</ul>

* * *