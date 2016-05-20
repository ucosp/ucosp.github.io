---
id: 1342
title: Detailed Update from WikiDev 2.0
date: 2009-11-19T15:39:50+00:00
author: eleni
layout: post
guid: http://ucosp.wordpress.com/?p=1342
permalink: /2009-2010/wikidev/2009/11/detailed-update-from-wikidev-2-0/
categories:
  - WikiDev
---
# Holly

### Status

  * Got arrows drawing between the nodes in the graph, not just lines.

**Roadblocks**

  * Arrows draw to the center of the nodes, not the edges

**Next Steps**

  * Get arrows to draw to node edges
  * Add documentation for the UI

# Eric

### Status

  * Currently working on adding queries to the backend to support the information needs of the frontend. 
      * Added support for querying all packages as well as by snapshot ID.
  * Also, working on changes to the parser as needed.
  * My priority this week is 1) documenting recently added queries, and 2) fixing parser bugs recently found.

<a name="Roadblocks"></a>

### Roadblocks

  * None at the moment.

<a name="Next_Steps"></a>

### Next Steps

  * Document new backend queries.
  * Fix parser bugs found by Brendan.
  * Talk to the front-end team to find out what they still need done.

# Alex

**Status**

  * Finish assigning different color and sharp to each relationship
  * Upload the new demo to the server (<a title="http://hypatia.cs.ualberta.ca/ucosp/extensions/WikiDev/UMLDisplay/bin-debug/WikiMapFlexProject.html" rel="nofollow" href="http://hypatia.cs.ualberta.ca/ucosp/extensions/WikiDev/UMLDisplay/bin-debug/WikiMapFlexProject.html">http://hypatia.cs.ualberta.ca/ucosp/extensions/WikiDev/UMLDisplay/bin-debug/WikiMapFlexProject.html</a>)
  * Improve the presentation of the UML graph
  * let class lead to the wikipage of the class

**Roadblocks**

  * No artifact info (still&#8230;.)

**Next Steps**

  * adding process bar (necessary if the parsing will take a long time)
  * continue improve the representation of graph

# Owen

### Status

  * Made a few improvements/bug fixes to the tree view in the Object nodes
  * Added custom icons to the tree view
  * Figured out how to put URL links on the graph
  * Started to play around with how to handle many nodes at once 
      * Partially implemented one idea

### Roadblocks

  * none

### Next Steps

  * Investigate why the parser is not handling method return types properly
  * Look into the license for Eclipse to see if we can actually use the icons I copied from it
  * Continue working on the graph appearance and the handling of many nodes at once

# Botlhale

### Status

  * Analyzing the results returned from queries to see if they match what is expected
  * Found issues with the results that were returned by the code and bugs were entered for the issues
  * Modified most of the code as the results did not entirely conform to what is expected
  * Updated team documentation page to indicate the completed and pending tasks and the strategies that were followed or will be followed to resolve the tasks and gave an example of different queries that are accomplished by the code.

**Next Steps**

  * Design queries to be able to return methods and fields return types
  * Start designing queries to query using the snapshot id
  * Collaborate with the flash team for additional interface resolutions in the next stages of the project
  * Keep updating the team documentation page as tasks get completed
  * keep analyzing returned XML results and possibly find bugs and fix in them

**Roadblocks**

  * Other school projects