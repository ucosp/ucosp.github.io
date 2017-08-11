---
title: Projects (January 2017)
author: ucosp-steering
layout: default
---
### Overview

We have an excellent list of projects, and I'd like to thank all the project mentors for taking the time to work with our students.

### September 2017

  * **Review Board:**
  * **UMPLE:**
  * **Firefox Code Coverage**
  * **Firefox React Debugger**
  * **Firefox Developer Tools - Inspector inline editor wigets**
  * **TaskCluster-CLI**
  * **Formulize**
    
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
  
### Firefox  React debugger

Last year, the [Firefox Debugger](https://github.com/devtools-html/debugger.html/) team decided to re-write the UI on Github with React. Today it has a modern web stack (React, Webpack, Babel) and is one of the most widely contributed to Mozilla projects. 

With this project, we want to take the next step and build on our relationships with the major framework and library teams to build the kind of tools that we would have liked to have while building the Debugger. We hope that these integrations will make the debugger feel more like a React or Ember debugger than a JS debugger.

Some examples of framework and library integrations include:

1. Highlighting framework frames in the call stack. 
2. Showing framework components in the source tree.
3. Previewing library objects on hover.

Highlighting framework frames in the call stack will let us tell the user what frameworks are doing when the application pauses. For instance, if the user pauses while making an API call, the debugger call stack can show the user that the application is updating the user record because the “save” button was pressed.

Showing framework components in the source tree will let users see their application’s framework types. In the case of React and Redux that includes (Components, Actions, and Stores). We think this view can be more valuable than just seeing source files because it is closer to how developers think about their applications. It also provides us a way to link to other framework information in the future. 

Previewing library objects will let frameworks format the objects the way they were intended to be seen. For instance, the most important data in a React component is the props and state. We hope to give frameworks control over how users see their framework objects because we think it paves the way for future integration points in the future. 

These features are exciting because it shows that when we work closely with libraries and framework teams, we can build new types of tools that help developers every day.



### Firefox Developer Tools - Inspector inline editor widgets

[Firefox Developer Tools](https://developer.mozilla.org/en-US/docs/Tools) (DevTools) allow developers to inspect and debug their web applications. The DevTools are built using web technology such as HTML, CSS and JavaScript utilizing the latest web libraries such as React and Redux.

In the Inspector, we will be working on a number of tools related to various CSS properties, Layout and Font inspection. Some examples of these new tools and features that previous students have worked on included:
CSS Grid Inspector
Box Model Layout panel improvements
CSS Variables Inspection
To read about some of the accomplishments from previous UCOSP students, visit https://hacks.mozilla.org/2017/06/new-css-grid-layout-panel-in-firefox-nightly/.

For the Inspector, we want to continue to working on better CSS Layout tooling such as CSS Grids and z-index inspector. In addition, we are aiming to implement more visual editors that will help developers and designers with debugging and editing complex CSS properties visually. Since CSS is very declarative by nature, we can provide tools that are commonly found in digital design tools, such as Adobe Photoshop and Illustrator, and Sketch, in order to bridge the learning gap of new developers and designers learning CSS. This would allow them to edit various CSS properties such as box-shadow, clip-path, gradient, filters, etc without knowing what the properties are.

Our goal is to help developers and designers come into the Inspector and be able to easily edit and learn HTML and CSS, and make changes to their web pages and eventually provide better authoring tools to help them also extract these changes.


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
  
