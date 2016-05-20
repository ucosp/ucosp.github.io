---
id: 1229
title: WikiDev Team Progress Report (week of Nov 2)
date: 2009-11-07T16:39:10+00:00
author: eleni
layout: post
guid: http://ucosp.wordpress.com/?p=1229
permalink: /2009-2010/wikidev/2009/11/wikidev-team-progress-report-week-of-nov-2/
categories:
  - WikiDev
---
# Alex

**Status**

  * Finish the UI part of history query
  * The graph can handle multiple classes

**Roadblocks**

  * The server cannot generate XML including the method and fields info for the related class

**Next Steps**

  * Finish navigation part
  * Change the PHP to accept our URL request

# Holly

**Status**

  * Cleaned up UI and code some
  * Added filter for Artifacts, set up structure to make it easier for later filters.

**Roadblocks**

  * Current visualization backend doesn&#8217;t easily support adding arrows on the lines, hindering making the graph look more UML-like. Looking for examples of how to override the default behavior, but not easily found.

**Next Steps**

  * Now that we have real data, make the graph look better with that &#8211; accommodate large numbers of field/methods, get them to fit on the screen better etc.

# Owen

**Status**

  * Co-ordinated with Brendan to get the SchemaSpy-generated files web-accessible
  * Read through both team SFU&#8217;s and Botlhale&#8217;s code in SVN to get up to speed on what they have done and prepare for switching teams
  * Also read through previous IRC discussions regarding the interface between the front and back ends
  * At our weekly meeting, I decided to join the front-end team.

**Roadblocks**

  * none

**Next Steps**

  * Discuss with Alex and Holly what our current tasks are, and how we will divide them up
  * Start contributing code to the front-end

# Botlhale

**Status**

  * Cleaning up unnecessary code from the repository
  * Synchronizing the code I have written with the rest of the project
  * Devising queries to include more details such as methods and fields in Object Object Relationship objects in the returned XML to be used by the flash team
  * Entered 3 bugs after analyzing the XML results returned

**Next Steps**

  * Do a research about the php get method in order to be able to use it without any security risks since the flash team prefers that it is used to pass the query values
  * continue working on queries to return methods and fields for objects in the object object relationships tag
  * resolve the bugs on the returned XML results
  * Collaborate with a team member who will be joining my team to divide tasks
  * Transforming the PHP code to have the methods getClasses() and getClassDetails(), initially designed the PHP code procedurally
  * Write SQL statements to query by pjsnapshotid
  * On verifying the SQL statement results, transform them into PHP to write the results in XML format that can be used by the flash team
  * Resolve any interface issues that might arise when writing code

**Roadblocks**

  * Midterms

# Eric

**Status**

  * I am moving to work on the back-end with Botlhale now.
  * My first priority this week is to try to get his php code integrated with the mediaWiki software. After that I will be updating it to allow for querying package hierarchies.

**Roadblocks**

  * Setting up a local copy of the wiki software to develop against &#8211; I&#8217;m especially dreading setting up postgreSQL.
  * With any luck, I can configure it to use the remote database.

**Next Steps**

  * Continue working on the parser in maintenance mode.
  * Add hook so mediaWiki can call Botlhale&#8217;s php files, so the front-end team can start testing against it.
  * Add ability for Botlhale&#8217;s script to report all the packages in the database. (From the most recent copy of each file? What happens for deleted files that have old versions in the database?)