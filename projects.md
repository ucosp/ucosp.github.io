---
title: Projects (September 2016)
author: ucosp-steering
layout: default
---
### Overview

We expect to add to this list over the next week or so, but here are the projects that are confirmed so far.

### September 2016

  * **Review Board:** Code review tool.
  * **Markus:** Web-based grading platform.
  * **UMPLE:** UML modeling and programming tool.
  * **Firefox Developer Tools - 3D Z-index Tool**
  * **TaskCluster-Pulse**
  * **Mylyn**
  * **Pontoon**
  * **Flyweb**
  
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

TaskCluster (https://docs.taskcluster.net/) is the task-execution
framework  that supports Mozilla's continuous integration systems.  It
runs tens of thousands of tasks per day, supporting the development of
Firefox and other Mozilla products.
TaskCluster is written in JavaScript, in the form of microservices
deployed in Heroku following the 12-factor guidelines.  All of the
services use a common set of internally-developed libraries, so they
all behave similarly, including accepting the same authorization
information.  The TaskCluster source code is (of course) open source
and available at https://github.com/taskcluster.

Pulse (http://pulseguardian.mozilla.org/) is an open message bus that
carries messages about all sorts of automated systems at Mozilla,
including detailed information about the status of Firefox builds and
tests.  TaskCluster uses pulse extensively behind the scenes.
PulseGuardian is a part of Pulse which allows anyone with an email
address to create credentials that allow reading and creating Pulse
messages.  However, these credentials are permanent and thus not
suitable for transient uses such as web-site users or ephemeral
computations.

The TaskCluster-Pulse project will implement a microservice similar to
PulseGuardian, but using JavaScript and the TaskCluster libraries.  It
will also involve some modifications to the TaskCluster tools site
(https://tools.taskcluster.net) to allow users to create new
credentials.  Beyond the capabilities of PulseGuardian,
TaskCluster-Pulse will allow creation of time-limited credentials
which disappear when they expire.

The UCOSP project will involve understanding the problem space,
proposing and agreeing on a design (including security concerns), and
then implementing that design.	
  
### Mylyn

[Mylyn's](https://www.eclipse.org/mylyn/) task-focused interface reduces information overload and makes multitasking easy. Mylyn makes tasks a first class part of the IDE, integrates rich and offline editing for ALM tools, and monitors your programming activity to create a "task context" that focuses your workspace and automatically links all relevant artifacts to the task-at-hand. This puts the information you need at your fingertips and improves productivity by reducing information overload, facilitating multitasking and easing the sharing of expertise.

Mylyn is written in Java and built on [Eclipse](http://www.eclipse.org/), and it's included in most Eclipse downloads, so students will have the chance to work on a tool that is downloaded over a million times every month! We have a number of projects for students to work on, including the following:
 
1. Task editor enhancements
  a. inline refresh as values change on the remote system
  b. provide a way to see the previous value of changed attributes, using the Eclipse compare framework to diff text attributes
  c. more frequent refresh of the active task
2. Mylyn context
  a. Improving the support for automated management of breakpoints as part of task context
  b. Providing a way to restrict a search to files in the task context
3. Improvements to the [Hudson/Jenkins](https://www.eclipse.org/mylyn/new/images/3.16/builds.png) connector which provides access to builds from CI systems from within Eclipse
4. Improvements to the Gerrit connector which provides access to Gerrit code reviews from within Eclipse

Students are also welcome to contribute their own ideas for consideration.

### Pontoon

[Pontoon](https://pontoon.mozilla.org/) is a localization tool by
Mozilla, designed for producing high quality translations. Its core
asset to support this goal is translation within the actual web
application, presenting real-time translation preview, context and
spatial limitations right in front of you.

To move translation quality support further ahead, we'd like to design
the translation review workflow that will:
  * help reviewers identify and categorize translation issues,
  * allow translators to learn from the received feedback from
translation reviewers and
  * empower team managers to evaluate performance and progress of their
team members.

At the core of this process will be the [Multidimensional Quality
Metric (MQM) standard](http://www.qt21.eu/mqm-definition/definition-2015-12-30.html#issue_types),
which is a framework for identifying and categorizing translation
issues. Your task will be to create a set of 4 different UX prototypes
of the translation review workflow in Pontoon.

By contributing to Pontoon, you will:
  * be taught how to design user interfaces to maximize the usability of
software product,
  * become familiar with the basics of web application development using Django,
  * learn programming through the educational code review process,
  * get to know the code hosting and version control platform GitHub and
  * track development progress in Bugzilla

Some experience using HTML, CSS, JavaScript, jQuery is required,
familiarity with Django or Python is a plus. You can learn more about
setting up the development environment in [developer documentation](http://mozilla-pontoon.readthedocs.io/en/latest/dev/install.html).

### FlyWeb

FlyWeb is an experimental new addition to the web platform that allows browsers to discover and connect to web servers (or application servers) that are near you.  FlyWeb also lets web pages to directly host web servers that are visible to other nearby browsers.

Our goal is to allow the web to let people interact with things and other people near them, without needing apps, or even a connection to the internet.  There are two classes of use cases that FlyWeb is targeted at:

1. User interfaces for smart devices.

As the number of smart devices grows, the problem of interacting with them increases.  Smartphone apps are currently the most common interface to these devices, but having a different app for every different thing you want to control doesn’t scale.  With FlyWeb, a smart device can simply advertise itself as a FlyWeb server, allowing browsers to discover and connect to it.  The UI for the device can be delivered as a standard web application via protocols such as HTTP and WebSocket.

The user doesn’t need to search for, download, and install apps just to interact with a new device.  They can just user their browser to discover and interact with it like they would an internet service.

2. App-less interaction between smartphones

FlyWeb lets web-pages publish their own discoverable FlyWeb servers.  This means that web pages can “extend themselves” between phones in a programmable way.

For example, a web game could expose a multiplayer mode which uses FlyWeb to start and publish a server.  When your friend discovers and connects to the game with their browser, the web page on your phone can send them a copy of the game code (the same as you received it from an internet server), and the two of you can play a multiplayer game without either of you having to download an app, or create an account, or tell each other your usernames, or any other coordination.

This mechanism can be extended to other interactions between people, like file-sharing, or shared whiteboards.

The UCOSP goal for the project is open-ended.  We want to see what ideas smart developers can come up with for applications that leverage the capabilities of FlyWeb.  Whether you want to build a smart device demo using Raspberry Pi, or a pure “browser to browser” demo using the web-page-publish-server feature, we want to see what you can come up with.

Your project, if successful, will be featured (given your permission) on our demo showcases, and potentially used to help promote the project.

Getting started is as easy as going to flyweb.github.io and following the instructions listed.
