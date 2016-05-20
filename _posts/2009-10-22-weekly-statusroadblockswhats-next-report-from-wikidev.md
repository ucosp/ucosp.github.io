---
id: 1038
title: 'weekly status/roadblocks/what&#039;s next report from WikiDev'
date: 2009-10-22T01:20:04+00:00
author: eleni
layout: post
guid: http://ucosp.wordpress.com/?p=1038
permalink: /2009-2010/wikidev/2009/10/weekly-statusroadblockswhats-next-report-from-wikidev/
categories:
  - WikiDev
---
## Eric

**Status**

  * Just finished building a test suite for the xmi parser.
  * See the testing plan for an overview of how it works.
  * The main body of the code lives in xmi parser/src/testsuite/testsuite.sh.
**Roadblocks**
  
Looking to the future, I&#8217;m not sure how to get ramped up on what Bolthale is doing &#8211; when the parser is done Team Waterloo is supposed to switch to helping him out. I need to get this figured out by next week.

**Next Steps**

  * Add suitable tests to the test suite as we go.
  * Work with Owen to do general cleanup of the code we&#8217;ve taken ownership of.
  
    Pushed back to this week when I took full ownership of the test suite.
## Owen

**Status**

  * Parsed associations into a separate DB table, storing the entity ID and multiplicity of each endpoint
  * Created a new test UML diagram and XMI file for associations using the 2 different aggregation types (composite and shared)
**Roadblocks**

  * The eUML plugin for Eclipse is somewhat buggy
**Next Steps**

  * Parse the aggregation type of each association endpoint
  * Create some test cases for the test suite
  * Clean up the Java code
  * Look into using the SchemaSpy tool (http://schemaspy.sourceforge.net/) for visualizing the JDEvAn database
## Alex

**Status**

  * Parse the sample XML file to get the information about Class and the relationship
  * Finish the basic rending for one Class, with methods, fields & artifacts (e.g. emails, articles and so on)
  * Clean up the code from previous application (wiki map)
**Roadblocks**

  * Need to find a way to represent the global structure for all the classes
  * Link all the info together to have a top-down view
**Next Steps**

  * Add the relationship between multiple classes
  * come up with standard URL request to get the real data
  * Integration with the server part
## Holly

**Status**

  * Discussed API to be used between Team SFU and Team UVic
  * Better idea of what WikiDev is doing &#8211; I keep thinking I have an idea, and then getting it updated. Progress!
  * Moving towards finalizing XML format
**Roadblocks**

  * Nothing, other than the usual scarcity of time.
**Next Steps**

  * Make it look more like a UML diagram &#8211; move methods/fields inside class definition
  * Make the node filters along the side work (goal to get it done today, but set the deadline for our next meeting)
## Botlhale

**Status**

  * Held an online meeting with team SFU to discuss the interface issues
  * Discussed about and designed an XML schema to be returned when searching using pjsnapshotid
  * Set up an environment to test PHP code (IIS and PHP) and verified it connects to the project server
  * Discussed how querying using pjsnapshotid can possibly be accomplished
  * Clarification on the expected API&#8217;s
**Next Steps**

  * Transforming the PHP code to have the methods getClasses() and getClassDetails(), initially designed the PHP code procedurally
  * Write SQL statements to query by pjsnapshotid
  * On verifying the SQL statement results, transform them into PHP to write the results in XML format that can be used by the flash team
  * Resolve any interface issues that might arise when writing code
**Roadblocks**
  
Failing to open an XML file input stream in a local environment setup to run PHP, issue to resolved by reading online articles