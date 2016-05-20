---
id: 2785
title: 'Guest post: an update from the POSIT project'
date: 2010-10-28T02:13:27+00:00
author: Andrew Louis
layout: post
guid: http://ucosp.ca/?p=2785
permalink: /fall2010/2010/10/guest-post-an-update-from-the-posit-project/
categories:
  - Fall 2010
tags:
  - POSIT
---
_[POSIT](http://posit.hfoss.org/) aims to create a portable, opensource tool for the Android platform to aid search and rescue efforts by allowing the transmission of data between users and to central servers. Mentor Ralph Morelli provided this update:_

Things are going very well with the POSIT group. The students have now all identified appropriate projects and each is making steady progress on their work. We have been meeting every Thursday for a brief Skype conference during which we discuss any issues that come up. The students have been very good about solving problems on their own and helping each other with ideas and suggestions. In addition they are also vetting each other&#8217;s bug fixes, which will help us resolve some of the outstanding issues.

Following is a brief summary of what the students in the POSIT group have taken on for their capstone projects. We will be tracking their contributions and their progress through POSIT&#8217;s issues tracker on the Google code repository. See issues 84-90 here: <http://code.google.com/p/posit-mobile/>

  * Edward Bassett ([Issue #84](http://code.google.com/p/posit-mobile/issues/detail?id=84)) will design and development an enhancement to the FindActivity that will directly allow the selected Find to be displayed on a Map. The Find will be centered on the Map. Edward has made several updates to the repository including to some of the tutorial (Wiki) pages. Edward has now acquired an Android phone and has done some good debugging of the Tracker module, which led to a bug fix in the repository.
  * Greg Knox ([Issue #86](http://code.google.com/p/posit-mobile/issues/detail?id=86)) will design and develop a search and/or sort feature to the ListFindsActivity. Similar to the search feature in the phone&#8217;s Contacts Activity, this will allow the user to more easily locate a specific Find within a long list of Finds. Greg has completed a good portion of the server-side implementation and is now working on the client side code.
  * Yang Ha ([Issue #87](http://code.google.com/p/posit-mobile/issues/detail?id=87)) will design and develop a fix a defect in the SyncFindsActivity whereby synchronization is not performed correctly on changes to finds after before T for Project A if that user had already synced the phone on Project B after time T. He has proposed a design for a revised Synchronization algorithm, which he is now implementing.
  * Derek Bachelor ([Issue #89](http://code.google.com/p/posit-mobile/issues/detail?id=89)) will design and develop a menu for the MapFindsActivity. Among other features, the menu will allow the user to center the map on the user&#8217;s current location or on a specific Find. Derek has proposed a nice design that includes several new features for the MapFindsActivity. He is now in the process of implementing them.
  * Anna Kournava ([Issue #90](http://code.google.com/p/posit-mobile/issues/detail?id=90)) will design and develop a Bluetooth based sync feature for the ListFindsActivity that will enable two phones to synchronize their Finds directly rather than by downloading them through the Server.