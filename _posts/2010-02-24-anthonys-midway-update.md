---
id: 2347
title: 'Anthony&#039;s Midway Update'
date: 2010-02-24T06:15:59+00:00
author: Anthony
layout: post
guid: http://ucosp.wordpress.com/?p=2347
permalink: /2009-2010/uncategorized/2010/02/anthonys-midway-update/
categories:
  - Ingres
  - Status
  - Uncategorized
---
Ingres support for Geotools has been progressing well. However, although we are already half way thru the term, we still have quite a ways to go, so we are beginning to pick up the pace a bit.

Comments and Observations:
  
&#8211; It seems like there is a lot of overhead and learning compared to the actually size of the code being developed. This has been a great learning opportunity, although it seems like given the learning curve, it would have been more effective if this project was longer than just one term.
  
&#8211; There was good communication within our team. This has been very important, as it has kept everyone up to date, motivated, and made sure that we were all on the right track. Weekly teleconference meetings have been very effective and I don&#8217;t feel that we have suffered from not being able to meet face to face.
  
&#8211; I came in with less experience with actually software development experience than other team members, so I spent a lot of my time bringing my skills up to speed (i.e. linux, svn, maven, etc). Again, this was a good learning opportunity for me.
  
&#8211; Lots of time spent writing status updates, reading mailing lists, reading emails, etc. This was a little surprising for me, but I soon realized how essential and beneficial communication and staying organized is. I particularly benefited from the knowledge of my teammates and mailing list participants.
  
&#8211; Lots of time spent installing and configuring supporting software.
  
&#8211; Our mentor, Andrew, has been very helpful in providing us with any required support.
  
&#8211; The average time put in per week was more than I had expected. After the first two weeks I realized I needed to put in at least 10 hrs per week to keep up. This has been very rewarding though, so no complaints!

Below are some of my status updates for the past few weeks.

Week of January 31st
  
What I&#8217;ve done this week:
  
&#8211; followed Lim&#8217;s instructions to set up debugging for GeoServer in Eclipse
  
&#8211; took a detailed look at the test classes proposed by Henry. I agree with his proposed action items.
  
&#8211; need to confirm whether skipColumnTest is necessary, my initial thought would be that it is
  
&#8211; spent a few hours trying without success to get the opengeo workshop to work with regards to writing data.. currently waiting for some help from geoserver mailing list
  
&#8211; having some problems with moving a school and then saving
	  
error msg: 06 Feb 15:31:41 ERROR [geoserver.ows] &#8211;
	  
org.geoserver.wfs.WFSException: Could not locate FeatureStore for &#8216;schools&#8217;

Week of February 7th
  
What I&#8217;ve done this week:
  
&#8211; got OpenLayers to write to postgis via Geoserver (using example code from opengeo workshop)
	  
issue was that table in query did not specify a workspace, and no default workspace was set. Upgraded to GeoServer 2.0.1 to be able to set appropriate default workspace
  
&#8211; mailed copyright form
  
&#8211; received SVN access
  
&#8211; continued reading GIS pdf

Week of February 14th
  
What I&#8217;ve done this week:
  
&#8211; import ingres project into eclipse
  
&#8211; read jdbc notes doc
  
&#8211; communicated with henry about test classes
  
&#8211; added 5 test classes