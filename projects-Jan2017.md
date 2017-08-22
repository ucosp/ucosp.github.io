---
title: Projects (January 2017)
author: ucosp-steering
layout: default
---
### Overview

We have an excellent list of projects, and I'd like to thank all the project mentors for taking the time to work with our students.

### January 2017

  * **Review Board:**
  * **UMPLE:**
  * **Firefox Code Coverage**
  * **Firefox Developer Tools - Inspector inline editor wigets**
  * **TaskCluster-CLI**
  * **Mylyn**
  * **Flyweb**
  
### Review Board

Review Board is a powerful web-based code review tool that helps developers do peer review as they write code. Review Board is used by thousands of software companies including Twitter, Yahoo, and VMware, as well as many open-source projects like Apache and KDE.
  
Students working on Review Board will have the opportunity to learn about back-end web development using Python and Django, as well as front-end development using HTML, CSS, Javascript, jQuery, and Backbone.js. Source control is managed via Git on GitHub. All patches are reviewed using Review Board, and students are expected to contribute to reviews for each other, as well as to other members of the development community.
Some possible projects include:

  * Making improvements to Review Board's extensions infrastructure, which allows third party developers to build features that aren't generic enough to be part of the product.
  * New kinds of integration with other services, such as deeper bug tracker integration, an adapter for GitHub pull requests, or allowing users to log in using Mozilla Persona.
  * Reworking parts of the UI to work better on touch devices like tablets and smartphones.
  
For a full list of project suggestions, check out our wiki:[Student Project Ideas](http://students.reviewboard.org/projects)

Some experience using Python and/or Django, Javascript and jQuery would definitely be a plus. In our experience, Git is usually the largest stumbling block, so students comfortable with Git (or able to quickly get comfortable with Git) will likely have an easier time developing.

For more information, see the project web page at <http://reviewboard.org>, or our students demo videos at <https://www.youtube.com/channel/UCTnwzlRTtx8wQOmyXiA_iCg/featured>



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

### Firefox Code Coverage

Code coverage can be used for many purposes. At Mozilla we have great ideas of how to use code coverage to better the quality of each version of Firefox and to make developers job easier by providing more data and easier testing.  

We have two long term goals we would like see implemented: 

1. Run a code coverage run every day on our infrastructure (linux64 only) for all unittests and generate a report that can be compared against a previous report. 
   * Customer: Release Management will use this to spot trends of increased or decreased coverage by module (top level directory in the source tree) and work with module owners/managers to understand risks and plan future work. 
2. Collect code coverage per test for each of the unittests we run and store the data in active data. 
    * Customer: Developers would be able to determine what unittests they need to run based on the changes in their patch
    * Customer: Release Management will be able to see code coverage of a new patch that they are considering uplifting to a beta/release version of Firefox. 
 
For the purposes of the 2016 Fall UCOSP program we will start by delivering goal #1. In order to achieve this we will need to:
 
  * Ensure we can build and run Firefox with c++ code coverage built in (build work, taskcluster work)
  * Ensure we can collect coverage from all test suites and proper gcda and gnco files are generated (taskcluster work, harness work) 
  * Retrieve all coverage data files and merge them together into a single lcov report (taskcluster work, lcov toolchain work, possibly docker image work) 
  * Determine hosting requirements for storing nightly reports and hosting the data, and the optimal way to store/serve the data (webserver, database, activedata) 
  * Ensure we can easily compare one report to another to easily highlight differences (python script/tool, web interface) 
  * Ensure we have coverage data broken down by module- top level directory in the Firefox source tree. (validating data, organizing report/queries/storage) 
  * Schedule a nightly run of code coverage builds+tests in a scheduler (taskcluster)


### Firefox Developer Tools - Inspector inline editor widgets

[Firefox Developer Tools](https://developer.mozilla.org/en-US/docs/Tools) allow developers to inspect and debug their web applications. The Developer Tools (DevTools) are built using web technology such as HTML, CSS and JavaScript and you will have the opportunity to use the tools you are building to inspect the DevTools itself.

In this particular project, we will be working within the CSS Rules inspector, which allows developers to examine and modify the CSS of a selected DOM element in the page. We want to introduce “inline editors” - a toggleable panel within the Rules view that expands below a given css property that is being edited. For example, clicking on a color in the Rules view would expand an area below the property containing the color displaying the color picker widget as we know it today. In addition, we will be looking to update the color picker to include color palettes and contrast ratio.

We want inline editors to become a common user experience pattern for visually editing values in the Rules view while also providing additional contextual information while working with the CSS property being edited. The stretch goal of this project is to implement additional inline editor widgets into our tools for CSS properties such as CSS filters and gradients, and CSS variables.

Check out our [wiki](https://wiki.mozilla.org/DevTools) on how to start working with our codebase, and the design specs for the color inline editor widget (https://projects.invisionapp.com/share/9G5R8XCYZ#/screens/143217180). For more information, reach out to [:gl] on IRC. We hang out in the #devtools channel at irc://irc.mozilla.org/devtools.

### TaskCluster-CLI

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

Taskcluster is mostly configurable through configuration that is checked
into the source-tree of whichever project is being built by Taskcluster,
but some other settings are configured through a web interface 
(https://tools.taskcluster.net/). We would like there to be a command line
interface as well and that will be the project we propose for this semester.
Features of the CLI include (but are not necessarily limited to):
triggering builds from various github branches
adding artifacts generated by builds to a queryable index
signing artifacts with a secret from our secrets service
auto-updating install from our artifacts
one-click-loaner/interactive-shell (https://docs.taskcluster.net/tutorial/debug-task) creation	
  
### Mylyn

[Mylyn's](https://www.eclipse.org/mylyn/) task-focused interface reduces information overload and makes multitasking easy. Mylyn makes tasks a first class part of the IDE, integrates rich and offline editing for ALM tools, and monitors your programming activity to create a "task context" that focuses your workspace and automatically links all relevant artifacts to the task-at-hand. This puts the information you need at your fingertips and improves productivity by reducing information overload, facilitating multitasking and easing the sharing of expertise.

Mylyn is written in Java and built on [Eclipse](http://www.eclipse.org/), and it's included in most Eclipse downloads, so students will have the chance to work on a tool that is downloaded over a million times every month! We have a number of projects for students to work on, including the following:

1. Improvements to the Task editor which allows users to read and edits tasks from various task repositories like Bugzilla.
2. improvements to Mylyn Task Context which tracks what files a user is interacting with when working on a task.
3. Improvements to the [Hudson/Jenkins](https://www.eclipse.org/mylyn/new/images/3.16/builds.png) connector which provides access to builds from CI systems from within Eclipse
4. Improvements to the Gerrit connector which provides access to Gerrit code reviews from within Eclipse

Students are also welcome to contribute their own ideas for consideration.



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
