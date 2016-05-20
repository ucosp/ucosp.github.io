---
id: 2206
title: Small Update
date: 2010-01-30T03:24:16+00:00
author: Brenda Sadoway
layout: post
guid: http://ucosp.wordpress.com/?p=2206
permalink: /2009-2010/eclipse4edu/2010/01/small-update/
categories:
  - Eclipse4Edu
---
<!--             HTML{height:100%;cursor:text;} BODY{padding:3px;border:0px;margin:0px;} .PlainText,.HTML{font-family:'Lucida Console' !important; font-size: 80%;} P{margin:0em !important;padding:0em !important;} BLOCKQUOTE,UL,OL{margin-top:0em !important;margin-bottom: 0em !important;padding-top:0em !important;padding-bottom:0em !important;} *{text-indent:0in !important;} SPAN.squiggly{border-bottom:dotted 1px #f00}          -->After our conference call today, here&#8217;s a summary of the current situation of what I&#8217;ve been working on, as well as the direction this aspect of the project is going:

The past couple weeks, I&#8217;ve been working on hiding references to packages (in the project explorer, as well as buttons and menus that allow the user to create a new package).

The concept that is being discussed is that we don&#8217;t want the user to work in Java Lite for the first month or so of their course, then come to the point where they switch to the regular Java perspective and become overwhelmed by the sudden presence of many tools they have not been introduced to.

Idea 1: Divide the Java Lite perspective into levels (beginner, intermediate, etc&#8230;) that determine which tools and aspects of Eclipse or visible and which are still hidden.  The user would be able to choose their level depending on what they feel comfortable with at the time.  The possible levels would be available through the welcome screen (and through a menu somewhere as well?).  There&#8217;s still the task of deciding what&#8217;s considered a basic tool meant for &#8220;beginner&#8221; users, what&#8217;s one step up from that, for &#8220;intermediate&#8221; users, and so on.

Idea 2: The program learns what should and shouldn&#8217;t be displayed over time based on the user&#8217;s activity.  If they are beginning to use certain tools, perhaps the next level of those tools, or others that might also be useful, should be visible from then on.  To avoid new aspects of the perspective suddenly appearing at seemingly random intervals, perhaps a window pops up when the user seems to be ready to learn about a new tool or concept, explaining where it is and what it&#8217;s used for (is this along the lines of a tutorial?).  Similar to Idea 1, there&#8217;s the task of deciding at what pace new tools are brought to the user&#8217;s attention, and in what order.  I think this would be based on what the user is already using, and how often.

Based on Idea 2, Wayne proposed in Bug 299965 that the default package should always be hidden.  If the project has an explicitly made package though, it should be visible.  Likewise, if only one source folder is present, it should be hidden, but if more than one exist, they should be visible as well.  This is to preserve the project structure the user or someone else (for example, a teacher), may have intended, while still simplifying the hierarchy where possible.

That about sums up what&#8217;s been discussed on this topic.

The conference call replaced our weekly meeting this week.

-Brenda