---
id: 1173
title: Elmcity Meeting Minutes for Oct 30 2009
date: 2009-11-01T16:51:55+00:00
author: jorygraham
layout: post
guid: http://ucosp.wordpress.com/?p=1173
permalink: /2009-2010/elmcity/2009/11/elmcity-meeting-minutes-for-oct-30-2009/
categories:
  - ElmCity
---
On Friday, the Elmcity team had its weekly meeting, the minutes of which can be found [here](http://jorygraham.com/elmcity/2009-10-30.153659-0400EDT.html).

A summary of the things we covered:

We went over and finalized our [grading scheme](http://ucosp.wordpress.com/2009/10/30/marking-scheme-for-elmcity-project/), including exactly what functionality we hope to have achieved by the 29th of November.

In that vein, we&#8217;ve decided that our functionality will primarily be dictated by the ability to parse the pages brought up by our users [here](http://friendfeed.com/elmcity/92ef3b61/hey-everyone-team-over-in-elmcity-development), and secondarily by this [list](http://blog.jonudell.net/2009/07/07/strategic-choices-for-calendar-publishers/). There&#8217;s a lot of overlap between the two, but our focus is on the sites the current curators are interested in.

We&#8217;ve all been looking over the patterns that should be recognized by our general parser, and will report on them this week.

Finally, we discussed which approach should be taken for parsing based on two libraries available for python: [parsedatetime](http://pypi.python.org/pypi/parsedatetime/0.8.4) and [dateutil](http://labix.org/python-dateutil). Dateutil seems to err on the side of caution, choking on any non-datetime text; whereas parsedatetime can handle a really wide range, but will also return false positives. We&#8217;ll likely have to take a middle ground approach to our parsing, since human generated text is so unpredictable.