---
id: 2407
title: 'Status Reports: Feb 22, 2010'
date: 2010-02-26T16:38:15+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=2407
permalink: /2009-2010/eclipse4edu/2010/02/status-reports-feb-22-2010/
categories:
  - Eclipse4Edu
  - Status
---
## **Brenda**

### Status

  * Looked further into the use of plugin_customization.ini for setting the default perspective and it seems this file is created when we compile a standalone RCP App. Cory posted details on its use in Bug 299869.
  * Submitted bug reports 303425, 303426 and 303427, related to the Class and Package wizards.
  * Submitted a patch that alters my previous patch for hiding packages and source folders so that all source folders are hidden, not just those named "src"
  * Looked into the other issue Wayne found with this patch (project explorer view not always updating), but haven&#8217;t come to a solution yet. 

### Next Steps

  * This week, continue to work on getting the project explorer view to update correctly. In particular, when a class is added under the specific circumstances mentioned by Wayne in Comment 8 on Bug 299965.

### Roadblocks

<ul type="disc">
  <li>
    None.
  </li>
</ul>

* * *

## **Cory**

### Status

  * Was on reading week, so had some extra time to put towards the project.
  * Started week looking into making the delete key work in the LitePackageExplorer (Bug 299875) and getting drag and drop (Bug 299878) to work. Found some good resources on implementing DND for eclipse plugin projects.
  * However, I followed Wayne&#8217;s advice on the delete key implementation, and have been mainly working on converting the delete menu item from LitePackageExplorer to use the built in delete Command (Edit->Delete). 
  * I have posted a couple patches for this &#8211; see Bug 299875 and Bug 303341.
  * Looked over Mile&#8217;s proposed patches for adding java source code templates to the java class constructors (Bug 302236). 
  * Added my comments to the thread, and also proposed a new patch doing it a little differently. 

### Next Steps

  * Continue work on Menu Commands / Handlers (Bug 303428 / 303341).
  * Will try and get back to drag and drop soon (Bug 299878).
  * Also attempt to fix small things as I see them. 

### Roadblocks

<ul type="disc">
  <li>
    None
  </li>
</ul>

* * *

## **Miles**

### Status

  * Developed a few versions for the architecture of templates for new Class creation.
  * Created the 2 wizards for class creation – New Java Program and New Java Class
  * Cleaned up the Welcome screen so the link works properly.
  * Fixed the New Class Wizard dialog size bug so that the dialog is a normal size as opposed to overly larg.

### Next Steps

  * Continue refactoring if necessary the Class creation constructor and wizards.
  * Make is so the Package field in the Class creation wizard is only displayed if there are packages created in the workspace.
  * I would really like to start spending some time on figuring out how to simplify the menus and toolbars. This is such a big problem with the plug-in that it would be nice to get this fixed by the end of the semester.

### Roadblocks

<ul type="disc">
  <li>
    The next couple weeks are going to be busy with midterms and assignments.
  </li>
</ul>

* * *