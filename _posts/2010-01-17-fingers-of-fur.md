---
id: 2053
title: Fingers of Fury
date: 2010-01-17T20:15:19+00:00
author: evanstratford
layout: post
guid: http://ucosp.wordpress.com/?p=2053
permalink: /2009-2010/sprint/2010/01/fingers-of-fur/
categories:
  - Sprint
  - Thunderbird
---
It&#8217;s 2:30 pm on Sunday; a thick pallor persists over an unseasonably warm Toronto. For roughly 40 students from various Canadian and American universities, this marks the end of the UCOSP code sprint. Those of us working on Thunderbird have made progress on a number of bugs [tagged with student-project](https://bugzilla.mozilla.org/buglist.cgi?keywords=student-project;keywords_type=allwords;emailtype1=exact;emailassigned_to1=1;query_format=advanced;bug_status=UNCONFIRMED;bug_status=NEW;bug_status=REOPENED;email1=nobody@mozilla.org;product=MailNews%20Core;product=Thunderbird):

  * Zach Church is tackling Thunderbird&#8217;s handling of recently closed tabs as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=504122) and [here](https://bugzilla.mozilla.org/show_bug.cgi?id=500758).
  * Tim Miller is working on better integration with Windows 7 as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=515907) and [here](https://bugzilla.mozilla.org/show_bug.cgi?id=494137).
  * Marcel Guzman is improving the Activity Manager as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=476487) and [here](https://bugzilla.mozilla.org/show_bug.cgi?id=536048), and is also adding a keyboard shortcut for switching between message and header panes as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=502515).
  * Kefu Zhao is automatically inferring From: addresses for replies to mailing lists as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=461669).
  * Lindauson Hazell is resolving a bug where message-related menu items are enabled in non-message-related tabs, as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=495815).
  * Evan Stratford is adding support for vCard import/export in Address Book as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=79709).
  * Wei Xian Woo is implementing session restore for Thunderbird as reported [here](https://bugzilla.mozilla.org/show_bug.cgi?id=408338).

Not a bad start at all! As we continue to make progress this week, more detailed updates will surface over on the [Mozilla wiki](https://wiki.mozilla.org/Thunderbird/Students/StatusUpdates/2010-01-22). Some lessons from the weekend:

  * Thunderbird is massive, and the codebase can often feel like C written in C++: it&#8217;s peppered with gems like return codes and extra output parameters and pointers to C-style strings. Put briefly &#8211; this is not the code you saw in class. Deal with it.
  * It&#8217;s incredibly important to discard hubris in open-source development. Check your ego at the door; don&#8217;t be afraid to ask questions; understand that you will be wrong many times before you are right. On the other hand, IRC places hundreds of experts at your fingertips, and is therefore more powerful than almost any tool you could use.
  * Practical lessons: [pbranch](http://arrenbrecht.ch/mercurial/pbranch/), [ack](http://betterthangrep.com/), and [MXR](http://mxr.mozilla.org/) are your friends; [ctags](http://ctags.sourceforge.net/) is also quite useful. If you don&#8217;t understand what to do, look at code that does something similar. If you still don&#8217;t understand what to do, ask. When using [Mercurial](http://mercurial.selenic.com/), never forget: commit early, commit often.
  * Remember: [have fun](http://lindausonhazell.com/Lindausons_Index/Movie.html)! As in any creative endeavour, passion keeps you going.

As a final note: I&#8217;d like to thank gvwilson for organizing the code sprint, which has proven to be an amazing opportunity to meet other talented and motivated developers. Additional shout-outs are due humph and bwinton for remaining diplomatic throughout the torrent of confused questions, and for providing helpful answers in return.

Happy hacking!