---
title: Projects (September 2016)
author: ucosp-steering
layout: default
---
### Overview

We expect to add to this list over the next week or so, but here are the projects that are confirmed so far.

### September 2016

  * **Review Board: **Code review tool.
  * **Markus: **Web-based grading platform.
  * **UMPLE: **UML modeling and programming tool.
  
### Review Board

Review Board is a powerful web-based code review tool that helps developers do peer review as they write code. Review Board is used by thousands of software companies including Twitter, Yahoo, and VMware, as well as many open-source projects like Apache and KDE.
  
Students working on Review Board will have the opportunity to learn about back-end web development using Python and Django, as well as front-end development using HTML, CSS, Javascript, jQuery, and Backbone.js. Source control is managed via Git on GitHub. All patches are reviewed using Review Board, and students are expected to contribute to reviews for each other, as well as to other members of the development community.
Some possible projects include:

  * Making improvements to Review Board&#8217;s extensions infrastructure, which allows third party developers to build features that aren&#8217;t generic enough to be part of the product.
  * New kinds of integration with other services, such as deeper bug tracker integration, an adapter for GitHub pull requests, or allowing users to log in using Mozilla Persona.
  * Reworking parts of the UI to work better on touch devices like tablets and smartphones.
  
For a full list of project suggestions, check out our wiki:[Student Project Ideas](https://reviewboard.hackpad.com/Student-Project-Ideas-bWzTgtBtq9f)

Some experience using Python and/or Django, Javascript and jQuery would definitely be a plus. In our experience, Git is usually the largest stumbling block, so students comfortable with Git (or able to quickly get comfortable with Git) will likely have an easier time developing.

For more information, see the project web page at <http://reviewboard.org>, or our students blog at <http://reviewboardstudents.wordpress.com/>


### Markus

MarkUs is a web-based grading tool built with Ruby on Rails. The primary goal of MarkUs is to make it easy for graders to read and annotate students' code. Graders also fill in a marking scheme or rubric created by the instructor.  Annotations may be saved for later reuse.  Students submit their code using either the web interface or using standard Subversion tools, and can form their own groups when allowed by the instructor. We are also working towards completing and integrated testing infrastructure that allows students to run instructor created tests on their submission and get realtime feedback. This summer we have been working on adding a feature to allow students to review other students' work.

Students working on MarkUs will learn basic web application development technologies using Ruby and Rails. MarkUs is hosted on Github so students will become familiar with Git and the process we use when working on the code. Because MarkUs is used by several thousand students in more than 4 universities (on 3 continents!), we take code quality seriously. All code submissions go through a code review, so the first task that students are asked to complete is fixing a trivial bug so that they become familiar with the code review process. 

Students working on MarkUs need to be able to work in Linux either natively or in a virtual machine. As the fall term comes to a close, we are putting together a list of the next projects. More information: <http://markusproject.org/>, <https://github.com/MarkUsProject/Markus>, and the blog, <http://blog.markusproject.org/>

### Umple

Umple is an open source toolkit whose objective is to merge UML modeling and programming into a single activity. Umple can be used in several ways: It can be used as a textual language for UML. It can also be used as a programming-language pre-processor, allowing UML concepts like associations and state machines to be added directly to Java, C++, and PHP. In addition, Umple allows drawing UML diagrams online and generating code directly from those diagrams. It is the goal of the Umple team to have large numbers of programmers and modelers incrementally adopt Umple. The barriers to entry are low, since using Umple can be done in a minimal way, without disrupting the existing model or code. Umple is an open-source project hosted on Github. You will have the opportunity to learn some or all of the following:

  * Model-driven design using UML
  * Test-driven development using JUnit
  * Programming in Java, Umple, PHP, C++, and/or Javascript
  * Compiler design including parsing and code generation
  * Web site design (of the UmpleOnline tool)
  * Eclipse plugin development (of the Umple plugins)
  * A variety of other libraries and tools
  * Agile open source development with continuous integration

The exact set of skills you will employ depends on the task(s) you choose to work on. More information: <http://www.umple.org> Suitable student projects: <http://projects.umple.org>


### Firefox Developer Tools - 3D Z-index Tool

Firefox Developer Tools allow developers to inspect HTML pages to better understand and debug how the structure of a web page translates into an image on the screen. Ultimately the image that is rendered to the screen is 2d, but it is composed of a variety of elements on the screen including blocks of color, text, images, and video. Conceptually these elements can be represented as a 3d document where the z-index of each element determines its height in the space. The higher z-indexed elements end up blocking the elements with lower z-indexes. However, this can become more complicated with the different types of positioning like 'absolute', 'relative', and 'fixed' positioning. Users can quickly become confused and struggle with stacking elements correctly.

The goal of this project would be to create a tool that intuitively lets users understand this overlapping structure of their webpage by visualizing it in three dimensions. Firefox devtools used to have a 3d debugging tool called Tilt, but its focus was on showing the nesting structure of a webpage, rather than the z-index stacking behavior. That tool is also no longer shipped with the Firefox devtools as it does not support multiprocess Firefox.

Some resources:
Z-Indexing: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index
Tilt Add-on: https://addons.mozilla.org/en-US/firefox/addon/tilt/

### TaskCluster-Pulse

An API service to generate temporary pulse (https://pulseguardian.mozilla.org) credentials. TaskCluster services such as this one are written in JavaScript using several in-house libraries.	
  * mechanism for generating temporary pulse credentials
  * API service using that mechanism	
