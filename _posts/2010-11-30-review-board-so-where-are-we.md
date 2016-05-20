---
id: 2788
title: 'Review Board: &#8220;So, where are we?&#8221;'
date: 2010-11-30T00:41:21+00:00
author: Andrew Louis
layout: post
guid: http://ucosp.ca/?p=2788
permalink: /fall2010/2010/11/review-board-so-where-are-we/
categories:
  - Fall 2010
---
_Originally posted by Mike Conley on the [Review Board student blog](http://reviewboardstudents.wordpress.com/2010/11/26/so-where-are-we/)._

If you’ve been following this blog, you’ll know that the team has been working very hard on their projects.  But I’ll bet those status reports can be a bit cryptic sometimes.

So here’s my take on where we are so far, in no particular order:

  1. Hongbin has been working on an extension that will allow communication between Review Board and various bug-trackers.  Currently, his extension listens for events on Review Board (such as publishing a review request, publishing a review), and then alerts the appropriate issue/bug in the bug-tracker by posting a comment with a link to the review request.  Hongbin’s extension currently only works with Google Code projects, but will eventually be extended to other bug-trackers as well (Bugzilla, Github’s issue tracker, etc).
  2. Laila has put together a new version of the Windows Review Board installer.  The installer is responsible for making sure a Windows machine has everything it needs in order to get an instance of Review Board up and running.  Laila is also working on a project that will allow review requests to have files attached to them.
  3. Lindsey and Brendan have been putting together an impressive suite of client tools to interact with the new Review Board API.  The monolithic “post-review” script will, I believe, be eventually modified to use these scripts.  The scripts are also designed to be easily imported, so that developers can write their own tools to interact with Review Board.
  4. Lianne has been working on an extension that will give Review Board WebHook notification abilities.  This means that, when various events happen on Review Board, the extension can send a request to a remote server to trigger another action.  Example:  when a review request has been marked as submitted, the Webhook might signal a script that publishes a notification to Twitter, or to an IRC bot, or to an RSS feed, etc.
  5. Kevin has completed his “collapsible-reviews” project: for review requests with a long series of reviews/revisions, we can save on vertical screen real-estate by automatically collapsing the reviews that have been read.  Kevin has also implemented a one-click Ship-It function, which makes easy reviews even easier.  Kevin is now working on the designs for a new user profile page for Review Board.