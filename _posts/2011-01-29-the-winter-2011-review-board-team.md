---
id: 2797
title: The Winter 2011 Review Board Team
date: 2011-01-29T09:26:43+00:00
author: Karen Reid
layout: post
guid: http://ucosp.ca/?p=2797
permalink: /2009-2010/uncategorized/2011/01/the-winter-2011-review-board-team/
categories:
  - Uncategorized
---
The Review Board team is happy to welcome our new 2011 Winter UCOSP
  
students! We&#8217;re looking forward to another successful semester of
  
Review Board development. So, without further ado, I&#8217;d like to
  
introduce the Winter 2011 Review Board Team:

  * Steve Sutcliffe
  * Kahlil Amlani
  * Mengyun Kong
  * Crystal Lok Koo
  * Teresa Hume
  * Mark Striemer

So the UCOSP codesprint finished up last week, and a lot got
  
accomplished. Students arrived with a Review Board development
  
install all ready to go, so they were eager to grab some easy bugs and
  
dive into the code. Lots of questions and traffic flew across IRC (3
  
/ 4 of the project mentors were not at the sprint, but were idling in
  
an IRC chatroom answering questions). Our students also got familiar
  
with Review Board’s Git workflow, and learned how to submit patches.
  
And patches were submitted! At least one of those patches has already
  
been merged, and the rest are still under review.

The team also used the weekend to tentatively select what projects
  
they wanted to work on. The projects are as follows:

**A Post-Commit WebUI (Crystal, Mark)**

Review Board so far has been geared toward pre-commit review, where a
  
change is put up before it&#8217;s committed. Many users want to be able to
  
instead select a revision or set of files (it depends on the type of
  
repository) and put them up for review instead. We&#8217;d need a good UI
  
for doing this.

**Quick Search (Crystal)**

Unlike the full-blown search that searches all the fields and file
  
paths and reviews and such, we could have a simple &#8220;quick search&#8221; that
  
provides a search field (we&#8217;d use the one for the standard search)
  
and, while typing, drops down a list of possible matches. It would
  
search summaries, review request ID numbers, users, and review groups.
  
It&#8217;d be a much faster way of getting around the site at times. A lot
  
still would have to be figured out for this.

**Spell Checking within Source Code (Mengyun, Kahlil):**

When syntax highlighting is used for diffs, Review Board can know if
  
it&#8217;s looking at a comment or a string or whatever. We could run a
  
simple spell check on the words and mark ones that might be spelled
  
incorrectly. We&#8217;d probably also want some way of adding words to the
  
Review Board install&#8217;s dictionary, which means adding new API.

**Extension Development (Mark, Kahlil)**

We&#8217;ve been working on an extension framework for a while now. It&#8217;s
  
coming along, but additional work probably needs to be done. What
  
we&#8217;ve been doing in the past is having someone work on an extension
  
idea and making sure that our extension framework is set up to do it.

**Scalability Testing Tools (Steve)**

We could always use new ways to help test the product.

One thing that would be useful would be a script that could
  
auto-generate/populate a database with sample data. It should be
  
configurable to create a certain amount of review requests, reviews,
  
diffs, users, etc. I should be able to run it and tell it I want
  
100,000 review request, each with between 1 and 10 reviews, and 1 and
  
5 diffs, across 300 users, and get a database I can work with. It
  
would greatly help for scalability.

**Theme Support (Teresa)**

Make it easy to override the look and feel of the site. Admins should
  
be able to drop a set of template files, images, CSS files, etc. in a
  
directory and configure Review Board to use that. What exactly we want
  
would have to be discussed further. It&#8217;s easy to go overboard or do
  
too little on a task like this.

It was a very successful sprint, and we’re looking forward to an
  
equally successful semester!

Mike Conley