---
id: 2310
title: Eclipse4Edu Meeting Minutes
date: 2010-02-19T20:52:35+00:00
author: Brenda Sadoway
layout: post
guid: http://ucosp.wordpress.com/?p=2310
permalink: /2009-2010/eclipse4edu/2010/02/eclipse4edu-meeting-minutes-2/
categories:
  - Eclipse4Edu
  - Status
---
Meeting Minutes February 19<sup>th</sup>, 2010

Present: Cory and Brenda

Not present: Miles

**Brenda**

&#8211;          Fixed the patch to Bug 299965 to hide all source folders, not just those named “src”.

&#8211;          Is looking into the issue with the project explorer view not updating under the circumstances that Wayne brought up in that bug.  It could be that elements are being filtered out and the refresh code is looking at the same list of elements and thus doesn’t know the elements exist.

&#8211;          Looked at adding Java Lite to the list of perspectives in the menu (as per Bug 299869).  Didn’t make much progress, but found PerspectiveSwitcher#addPerspectiveShortcut, which might be a good place to look further for this issue.

**Cory**

&#8211;          Got the delete handler logic set up.  Wayne made a new bug for refactoring the delete action from the package explorer so that both the handler and explorer can run the same code.

&#8211;          We should be able to enable other global menu items doing something similar using XML.

&#8211;          Found good reference material for implementing drag and drop, but wants to finish what he’s working on with the delete functionality first.

&#8211;

**Miles**

&#8211;          Working on the creation wizards, in particular the templates.

**Other**

&#8211;          Cut, copy and paste: will need to create the logic to shuffle elements in the package explorer, which will tie in with drag and drop.

&#8211;          Some useful links Cory found:

  * Information on XML: [http://wiki.eclipse.org/Command\_Core\_Expressions](http://wiki.eclipse.org/Command_Core_Expressions)
  * Information on drag and drop: http://www.eclipse.org/articles/Article-Workbench-DND/drag_drop.html
  * Reference that covers just about everything: [http://wiki.eclipse.org/Eclipse\_RCP\_How-to](http://wiki.eclipse.org/Eclipse_RCP_How-to)