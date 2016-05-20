---
id: 2621
title: Thunderbird Update
date: 2010-03-10T04:01:42+00:00
author: wxwoo
layout: post
guid: http://ucosp.wordpress.com/?p=2621
permalink: /2009-2010/status/2010/03/thunderbird-update/
categories:
  - Status
  - Thunderbird
---
Some quick updates from the Thunderbird team for weeks starting February 22nd and March 1st. (This is a point-form summary; see <https://wiki.mozilla.org/Thunderbird/Students/StatusUpdates> for each week&#8217;s full report.)

**Tim (Bug: Windows 7 overlay icons &#8211; <https://bugzilla.mozilla.org/show_bug.cgi?id=515907>)**

  * Wrote a short guide on Mozilla&#8217;s patch development process
  * Corrected a few issues related to incorrect usage of data types in his XPCOM component
  * Submitted a patch
  * Investigated test frameworks appropriate for testing his Windows 7 overlay icons implementation &#8211; this is tricky because Mozilla has A LOT of test frameworks. It turns out that Tim needed to do mochitests and although these are tests for Thunderbird, they have to be run from Firefox.
  * Plans to submit test cases this week (week of March 8th)

**Kefu Zhao (Bug: automatically determine &#8220;From&#8221; address for &#8220;reply to list&#8221; &#8211; [https://bugzilla.mozilla.org/show_bug.cgi?id=461669](https://bugzilla.mozilla.org/show_bug.cgi?461669))**

  * Working on retrieving the raw headers of an e-mail (still in-progress)

**Wei Xian Woo (Bug: improved session storage and restoration in Thunderbird &#8211; <https://bugzilla.mozilla.org/show_bug.cgi?id=408338>)**

  * Received feedback about my first patch from Blake and made the suggested changes
  * Improved some test cases and added a new one
  * Made additional changes to the session store manager to make intentions more clear
  * Submitted revised first patch for review
  * Brainstormed ideas for implementing support for persisting session state for other window types (right now, we only persist session state for the main Thunderbird windows aka the 3-pane windows).

**Everyone else**

  * Still happily working on their respective bugs. Recap of what they are working on: 
      * Zach Church &#8211; &#8220;reopen last closed tab&#8221; (<https://bugzilla.mozilla.org/show_bug.cgi?id=504122>)
      * Marcel Guzman &#8211; interactive status bar/Activity Manager (<https://bugzilla.mozilla.org/show_bug.cgi?id=476487>)
      * Lindauson Hazell &#8211; all message related functions should go through default controller code (<https://bugzilla.mozilla.org/show_bug.cgi?id=495815>)
      * Evan Stratford &#8211; vCard import (<https://bugzilla.mozilla.org/show_bug.cgi?id=79709>)