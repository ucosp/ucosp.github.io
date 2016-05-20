---
id: 2245
title: Summary of the Week
date: 2010-02-05T21:00:34+00:00
author: Brenda Sadoway
layout: post
guid: http://ucosp.wordpress.com/?p=2245
permalink: /2009-2010/eclipse4edu/2010/02/summary-of-the-week/
categories:
  - Eclipse4Edu
  - Status
---
We had a meeting today at 2:00 PM Eastern Time.

Present: Cory and Brenda

Not Present: Miles (his computer broke)

Here&#8217;s what&#8217;s been going on:

**Brenda**

&#8211; Discussed possibilities in regards to hiding packages from the user.

&#8211; Looked into different ways of showing/hiding packages and posted another patch for Bug 299965 for use in comparing the alternatives.

**Cory**

&#8211; Discussed possibilities in regards to hiding packages from the user.

&#8211; Tried his first year assignments in Java Lite and sent an email to the mailing list on February 3, 2010 with results and suggestions regarding:

  * Importing existing projects into the workspace
  * Java Applets
  * Connecting multiple files for compilation
  * “Add main method” checkbox in the New Class Wizard
  * No use for source folders or packages at all

**Miles**

&#8211; Discussed possibilities in regards to hiding packages from the user.

&#8211; His computer broke during the week.

**Hiding Packages**

&#8211; We’re leaning towards hiding all references to packages based on personal experience in first year Java courses.

&#8211; Bug 299965 has two patches posted, one of which hides all packages, package buttons and the src folder.  The second only hides the default package and src folder (explicitly-made packages are visible).

&#8211; The idea of making packages visible after the user has gained some experience (ie, through making their own classes), was also brought up.  It was thought that this would be likely to cause confusion.

&#8211; Showing the “create a package” buttons might also cause confusion if default packages are hidden.