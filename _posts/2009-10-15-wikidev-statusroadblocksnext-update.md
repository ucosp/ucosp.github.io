---
id: 996
title: WikiDev Status/Roadblocks/Next Update
date: 2009-10-15T16:05:13+00:00
author: eleni
layout: post
guid: http://ucosp.wordpress.com/?p=996
permalink: /2009-2010/wikidev/2009/10/wikidev-statusroadblocksnext-update/
categories:
  - WikiDev
---
# Botlhale {#firstHeading.firstHeading}

<a name="Status" id="Status"></a>
  


### <span class="mw-headline">Status</span>

  * Discussed the way requests to the database are going to be made 
  * Agreed on the XML schema to be returned when requests are made 
  * Queried the database by use of entity id&#8217;s and managed to get information on objects and object relationships 
  * Learnt about writing XML files in PHP 
  * Wrote PHP code (The code is not yet verified to work as expected) to perform SQL commands in the database and use the results of the SQL Commands to write an XML file according to the given XML schema 
  * Introductory discussions with the Flash team about an interface with my code in order for them to be able to use the XML file returned to draw graphics 
  * Discussed about designing an API for the queries performed, initial thoughts were to have an API for methods getClasses() and getClassDetails() 

<a name="Next_Steps" id="Next_Steps"></a>
  


### <span class="mw-headline">Next Steps</span>

  * Setup a PHP environment to verify that the code written so far functions as expected 
  * Discuss about how the pjsnapshotid can be used as a variable to make requests to the database to get object information and how it will be used to retrieve data from previous versions of code 
  * Design the code so that we can have methods which will be defined in the API 
&#8211; Collaborate with the flash team to be able to have a design compatible with their design idea </li> </ul> 

<a name="Roadblocks" id="Roadblocks"></a>
  


### <span class="mw-headline">Roadblocks</span>

  * Having an environment to run PHP files 

<a name="top" id="top"></a>

# Eric {#firstHeading.firstHeading}

<a name="Status" id="Status"></a>
  


### <span class="mw-headline">Status</span>

  * My section of the parser is done for the moment (finished method parsing this week), so now until next week I&#8217;m working on building a testsuite for doing regression tests. 

<a name="Roadblocks" id="Roadblocks"></a>
  


### <span class="mw-headline">Roadblocks</span>

  * Nothing in particular right now other than finding the time to work on this. 

<a name="Next_Steps" id="Next_Steps"></a>
  


### <span class="mw-headline">Next Steps</span>

  * Finish building test suite. 
  * Work with Owen to do general cleanup of the code we&#8217;ve taken ownership of. 

<a name="top" id="top"></a>

# Holly {#firstHeading.firstHeading}

<a name="Status" id="Status"></a>
  


### <span class="mw-headline">Status</span>

  * Flex parses XML and displays graph &#8211; my version doesn&#8217;t show nodes, Alex&#8217;s does 

<a name="Roadblocks" id="Roadblocks"></a>
  


### <span class="mw-headline">Roadblocks</span>

  * Finding time between other classes, both to work and to collaborate 
  * Earlier, getting nodes displayed &#8211; since been solved by Alex in a different branch 

<a name="Next_Steps" id="Next_Steps"></a>
  


### <span class="mw-headline">Next Steps</span>

  * Reconciling differences between Alex&#8217;s and I&#8217;s code 

<a name="top" id="top"></a>

# Alex {#firstHeading.firstHeading}

<a name="Status" id="Status"></a>
  


###  <span class="mw-headline">Status </span>

  * Parse the sample XML file to get the information about Class and the relationship 
  * Finish the basic rending for one Class, with methods, fields & artifacts (e.g. emails, articles and so on) 
  * Clean up the code from previous application (wiki map) 

<a name="Roadblocks" id="Roadblocks"></a>
  


###  <span class="mw-headline">Roadblocks </span>

  * Need to find a way to represent the global structure for all the classes 
  * Link all the info together to have a top-down view 

<a name="Next_Steps" id="Next_Steps"></a>
  


###  <span class="mw-headline">Next Steps </span>

  * Add the relationship between multiple classes 
  * come up with standard URL request to get the real data 
  * Integration with the server part 

<a name="top" id="top"></a>

# Owen {#firstHeading.firstHeading}

<a name="Status" id="Status"></a>
  


###  <span class="mw-headline">Status </span>

  * Uploaded a sample XMI file with corresponding image to SVN 
  * Finished parsing template classes 
  * Finished basic parsing of associations 

<a name="Roadblocks" id="Roadblocks"></a>
  


###  <span class="mw-headline">Roadblocks </span>

  * none 

<a name="Next_Steps" id="Next_Steps"></a>
  


###  <span class="mw-headline">Next Steps </span>

  * Improve the handling of associations by using a new DB table 
  * Also parse the association endpoints 
  * Work on cleaning up the Java code