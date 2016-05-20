---
id: 2663
title: Markus March 19th Punchlines
date: 2010-03-19T19:38:45+00:00
author: Joseph
layout: post
guid: http://ucosp.wordpress.com/?p=2663
permalink: /2009-2010/markus/2010/03/markus-march-19th-punchlines/
categories:
  - MarkUs
tags:
  - MarkUs
  - meeting minutes
  - punchlines
  - Winter 2010
---
## Victoria

### Status

  * Brainstormed ideas for the Dashboard.
  * Went through draft Dashboard contents with Karen and Farah and got some good and constructive feedback

### Next Steps

  * With the feedback I got back regarding the potential Dashboard contents, come up with a preliminary prototype &#8212; one that we can take apart and help establish a better idea as to how we&#8217;d like to design the Dashboard.

### Roadblocks

  * Swamped with work (from my full-time position).

## Mike

### Status

  * Applied 0.6 patches to trunk
  * Also caught some missing translations and brought them over from 0.6
  * Reviewed a bunch of code
  * Email / IRC development support

### Next Steps

  * Same as always &#8211; review, review, review.  Answer email.  Help where I can.

### Roadblocks

  * None

## Farah

## Status

  * Finished implementing the ability for an instructor to release/unrelease the marks for grade entry forms
  * Submitted a review request (in two parts) for the student UI and releasing the marks (see <a href="http://review.markusproject.org/r/458" target="_blank">http://review.markusproject.org/r/458</a> and <a href="http://review.markusproject.org/r/459/" target="_blank">http://review.markusproject.org/r/459/</a>)
  * Modified the table view so that the text boxes for entering grades are smaller
  * Worked on unit tests for the student UI and releasing the marks and submitted a review request (see <a href="http://review.markusproject.org/r/473/" target="_blank">http://review.markusproject.org/r/473/</a>)

### Next Steps

  * Work on functional tests for the student UI and releasing the marks
  * Implement CSV upload/download for grade entry forms
  * Tests for CSV upload/download

### Roadblocks

  * None this week

## Joseph

### Status

  * Met with Mike on Tuesday to discuss how to test the server side pagination
  * renamed ajax pagination helper to pagination helper ( <http://review.markusproject.org/r/470/> )
  * migrate the submissions\_controller\_test from fixtures to machinist ( <http://review.markusproject.org/r/474/> )

### Next Steps

  * continue with the testing
  * finish of the suggestions from reviewers
  * get a start on the detailed submissions view

### Roadblocks

  * assignments

## Bryan

### Status

  * Wrote a draft version of user stories: assigning graders to criteria.
  * Introduce factory data preloader, which can be used in conjunction with Machinist and improve its speed. Modified the results\_controller\_test.

### Next Steps

  * Finish the class diagram and database schema for the feature &#8220;assigning graders to criteria&#8221;
  * Plan how to use single table inheritance to implement flexible and rubric criterion
  * Find a good pattern for factory data preloader

### Roadblocks

  * None

## Robert

### Status

  * The ability to create Notes on Assignments, and Students from the new notes page is complete and awaiting final approval.
  * Added tests for the new noteables to the Notes Controller Test
  * Converted Notes Controller Tests to Machinist
  * Added a Machinist blueprint for Notes.

### Next Steps

  * Add the notes dialog links to the Student pages and the Assignment pages.
  * Convert the Student and Assignment tests to Machinist and Shoulda.

### Roadblocks

  * None!

## Brian

### Status

  * Fix a small bug Ticket #622
  * Working on refactoring database, doing some test
  * Improving flexible schemes

### Next Steps

  * make flexible scheme ready to ship
  * make prototype of new database design

### Roadblocks

  * none