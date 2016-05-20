---
id: 2800
title: CoRAL progress this week
date: 2011-02-04T10:53:18+00:00
author: Karen Reid
layout: post
guid: http://ucosp.ca/?p=2800
permalink: /2009-2010/uncategorized/2011/02/coral-progress-this-week/
categories:
  - Uncategorized
---
After the code sprint, from Jan 27-Feb 03, we continued to become more familiar with the code base, and began working on implementing some of the core features of CoRAL. These features include the authentication of users, and the uploading of publications. A new login page was created, which will allow users to log in and out of the site. Ultimately this will restrict the functionality on the website (such as uploads) until a user has logged in.

The user profile was also updated by implementing the &#8216;publications&#8217; tab. This displays all the publications that that particular profile/user is considered an author of. A link was created to facilitate the upload/claim of a user&#8217;s publication.  This provides the user with a form to fill out their paper&#8217;s information such as title/author/DOI etc. It also provides an optional file upload if the user wishes to upload a copy of the paper. This week, the UI portion of the upload was completed, and next week we will work on implementing the upload of a file/writing a publication record to the database.

A number of minor changes were also made to the application, such as changing the color of the communication network, and reordering the UI elements that appear on a paper&#8217;s &#8216;profile&#8217; page. This upcoming week we also hope to implement the &#8216;settings&#8217; tab for a user&#8217;s profile, as well as tweak the implementation of the publication uploading. We also wish to allow a user to &#8216;claim&#8217; authorship over a paper on the site.

&#8212; Adam Williams