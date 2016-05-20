---
id: 971
title: Elmcity Status Reports for 2009-10-14
date: 2009-10-14T15:43:55+00:00
author: jorygraham
layout: post
guid: http://ucosp.wordpress.com/?p=971
permalink: /2009-2010/elmcity/2009/10/elmcity-status-reports-for-2009-10-14/
categories:
  - ElmCity
  - Status
---
I haven&#8217;t heard back from the whole team, but here are the status reports I did receive:

**Jory**

Status:

  * Implemented the SQL layer in database.py by&#8230;
  * Restructuring and refactoring icsWriter.py and remote.py

Roadblocks:

  * We don&#8217;t have any unit or integration tests, so it&#8217;s impossible to be completely reassured with code changes.

Next Steps:

  * Write integration tests for database.py?
  * Write unit tests for remote.py
  * Further restructuring of remote.py

**Diane**

Status:

  * Still working on cataloguing what sorts of general patters we should support.  Expect to have results by the end of the week.
  * Setting up Cathy Levinson&#8217;s elmcity wordpress plugin (Calendar Display Mechanisms) and investigating how to divide the work between the elmcity service and the plugin.

Roadblocks:

  * None.

Next Steps:

  * Continue working on the cataloguing of general patterns found within existing FuseCal-parsed pages.  Expect to have results published by the end of the week.
  * Look into how the elmcity wordpress plugin is sourcing JSON and how client-side rendering directly in the elmcity service might be more useful and how it may not be.

**Nikita**

Status:

  * Wrote remote.py
  * Implemented bad_urls table
  * Wrote up about the project page, with simple instructions on how to use the service
  * Restructured hg repository so that it&#8217;s now mirror of our server structure
  * Updated ajax interface & frontend so it doesn&#8217;t choke on malformed URLs

Roadblocks:

  * None

Next Steps:

  * Add filter capability to the service
  * Write-up &#8220;how to write a plugin&#8221; plugins guidelines
  * Write batch processing module

**Sarah**

Status:

  * I&#8217;m looking into Autopager, a firefox plugin that does a very good job of allowing users to generate rules to select different parts of a page.
  * I&#8217;m reading through the source code and sketching out some ideas as to how a plugin generator for us would look, how to make the interface more usable, and what extra features we&#8217;d need.

Roadblocks:

  * Waiting for answer from developer of whether Autopager is free for reuse with modification, or just open source
  * I&#8217;m not entirely sure whether this side project is a good use of team resources: Would a complementary generator to Diane&#8217;s project be worthwhile?

  * I was trying to wait until I had something more concrete to blog about it, but I could really use some input from the rest of the team

Next Steps:

  * I&#8217;ll put together a UCOSP Elmcity ics with the meetings, this weekly post, and other events &#8211; if nothing else, it&#8217;d help me stay on top of things.

  * I&#8217;ll make a blog post about this idea, and solicit opinions from the rest of the group.
  * Search for and blog about the question: what is fair use for open source but not free software? Can I dissect Autopager&#8217;s approach in detail, throw away their code, and write from a guideline I got from their source? Can I look through Autopager&#8217;s source when I hit a design problem, and implement their solution &#8220;in my own words&#8221;? Or am I not really allowed to make what would be conceptually a derivitive work if I&#8217;ve read their code? I&#8217;m sure a lot of people working on UCOSP could help me with this.