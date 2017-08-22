---
title: Projects (January 2017)
author: ucosp-steering
layout: default
---
### Overview

We have an excellent list of projects, and I'd like to thank all the project mentors for taking the time to work with our students.

### September 2017

  1. **Review Board:**
  2. **UMPLE:**
  3. **Firefox Code Coverage**
  4. **Firefox React Debugger**
  5. **Firefox Developer Tools - Inspector inline editor wigets**
  6. **TaskCluster Resource Monitoring**
  7. **Formulize**
  8. **WALA Program Analysis for Swift**
  9. **Safe Browsing and Tracker Prevention**

---     
### 1. Review Board

Review Board is a powerful web-based code review tool that helps developers do peer review as they write code. Review Board is used by thousands of software companies including Twitter, Yahoo, and VMware, as well as many open-source projects like Apache and KDE.
  
Students working on Review Board will have the opportunity to learn about back-end web development using Python and Django, as well as front-end development using HTML, CSS, Javascript, jQuery, and Backbone.js. Source control is managed via Git on GitHub. All patches are reviewed using Review Board, and students are expected to contribute to reviews for each other, as well as to other members of the development community.
Some possible projects include:

  * Making improvements to Review Board's extensions infrastructure, which allows third party developers to build features that aren't generic enough to be part of the product.
  * New kinds of integration with other services, such as deeper bug tracker integration, an adapter for GitHub pull requests, or allowing users to log in using Mozilla Persona.
  * Reworking parts of the UI to work better on touch devices like tablets and smartphones.
  
For a full list of project suggestions, check out our wiki:[Student Project Ideas](http://students.reviewboard.org/projects)

Some experience using Python and/or Django, Javascript and jQuery would definitely be a plus. In our experience, Git is usually the largest stumbling block, so students comfortable with Git (or able to quickly get comfortable with Git) will likely have an easier time developing.

For more information, see the project web page at <http://reviewboard.org>, or our students demo videos at <https://www.youtube.com/channel/UCTnwzlRTtx8wQOmyXiA_iCg/featured>

---

### 2. Umple

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

---

### 3. Firefox Code Coverage

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
 
 ---
  
### 4. Firefox  React debugger

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

---

### 5. Firefox Developer Tools - Inspector inline editor widgets

[Firefox Developer Tools](https://developer.mozilla.org/en-US/docs/Tools) (DevTools) allow developers to inspect and debug their web applications. The DevTools are built using web technology such as HTML, CSS and JavaScript utilizing the latest web libraries such as React and Redux.

In the Inspector, we will be working on a number of tools related to various CSS properties, Layout and Font inspection. Some examples of these new tools and features that previous students have worked on included:

* CSS Grid Inspector
* Box Model Layout panel improvements
* CSS Variables Inspection

To read about some of the accomplishments from previous UCOSP students, visit https://hacks.mozilla.org/2017/06/new-css-grid-layout-panel-in-firefox-nightly/.

For the Inspector, we want to continue to working on better CSS Layout tooling such as CSS Grids and z-index inspector. In addition, we are aiming to implement more visual editors that will help developers and designers with debugging and editing complex CSS properties visually. Since CSS is very declarative by nature, we can provide tools that are commonly found in digital design tools, such as Adobe Photoshop and Illustrator, and Sketch, in order to bridge the learning gap of new developers and designers learning CSS. This would allow them to edit various CSS properties such as box-shadow, clip-path, gradient, filters, etc without knowing what the properties are.

Our goal is to help developers and designers come into the Inspector and be able to easily edit and learn HTML and CSS, and make changes to their web pages and eventually provide better authoring tools to help them also extract these changes.

---

### 6. Mozilla Taskcluster Resource Monitoring and Management

The [Taskcluster](https://docs.taskcluster.net/) team at Mozilla builds a platform for performing the continuous integration of the Firefox web browser.  We currently perform many of our operations using cloud resources, primarily the AWS suite of tools.  We would like to expand our monitoring and management of our AWS resources.  The first area we’d like to focus on is EC2 (VMs as a service).

We have a component that manages our EC2 account called ‘ec2-manager’.  In this service, we’d like to monitor things like how many instances we have, how many spot requests are open and how many EBS volumes we have.  We’d like to feed that into our standardized reporting tool called ‘statsum’ so that we can spot trends and highlight issues.

We’d also like to have tools to monitor for unused resources which cost us money or are causing our account to be messy.  Examples are reporting on machine images (AMI) snapshots which haven’t been used in a long time, EBS Volumes which aren’t attached to anything and SSH key pairs.

A third thing we would like to do is monitor the reasons for instance termination and spot request outcomes.  This can be used to gather information on the health of EC2, since the Amazon provided means of determining health are incomplete.

The final component would be to introduce management of resources.  The main resource here is Security Groups for EC2 instances.  These are a white list based set of firewall rules which can be attached to EC2 instances.  We’d like to have facilities for automated management and monitoring for them.  We would like to have checks in place to ensure that we are alerted if any changes from the expected security group settings are made.

Students for this project should be familiar with Javascript in the Node.js environment.  We are using the native async function support included in recent versions of Node.js, but other parts of our platform are implemented using Babel for transpilation.  The main service we’re working with uses a Postgres SQL Database.

---

### 7. Formulize

Formulize is a tool for making data management systems on the web. 

Formulize has extensive support for modelling workflows, so that organizations can customize how users interact with the data that Formulize is managing. It is aimed at “power users” in not-for-profits and other organizations without large IT departments and resources, empowering them to create systems that would otherwise require custom programming to deploy. 

The most basic operation in Formulize, is the creation of forms. Administrators can specify what elements should appear on the form, and also how different groups of end users should be able to interact with the form. From there, administrators can make custom screens that control how lists of entries in each form are shown to end users. 

Administrators can also control how different forms relate to each other, similar to describing table relationships in an ERD. These relationships then govern how data is queried from the database, enabling screens to display complex sets of information to users, rather than just entries from a single form. 

Formulize can work as a standalone application, installed on a web server. Formulize can also be embedded within any PHP-driven web application on the same server where it is installed. A Drupal module has been created that supports extensive integration with the Drupal content management platform, including single sign-on for users. Integration plugins for WordPress and Joomla have also been created (by previous UCOSP students!). 

#### Who uses Formulize? 

Formulize is used by organizations around the world, for a variety of purposes, from tracking the status of housing renovations, to recording the activities of wilderness rescue teams. Formulize was created by Freeform Solutions, a Canadian not-for-profit organization that helps other not-for-profits with IT. 

#### How is Formulize built? 

Formulize is built primarily with PHP, but makes use of HTML and Javascript as well of course. jQuery is also used extensively in the more recent parts of the code base (the project started in 2004). Formulize relies on MySQL for database operations. 

Because it is a tool that you use to create other systems, rather than a tool that does something for end users by itself, there is a high degree of abstraction throughout the codebase, especially the parts that interact with the database. The code has to read configuration information specified by the administrators, and use that to dynamically generate all operations, including database queries. 

The newer parts of the codebase employ some object orientation. Older parts remain largely procedural. The codebase is maintained on GitHub. 

#### What will students learn? 

Students will have extensive exposure to PHP of course, and related web technologies. This term, we will begin by focusing on upgrading Formulize to be compatible with PHP 7. There are also several significant, older branches that are complete, but need updating to merge into the current master branch. 

Over the years, Formulize has developed a specific process for managing code, tests and documentation all through our GitHub repository. Our the tests are run automatically by a continuous integration system, based on Travis-CI and Sauce Labs. Students will have exposure to this entire process as part of contributing to the Formulize project. 

Learn more about Formulize: 

Download Formulize and docs: http://formulize.org/formulize-downloads

Browse the GitHub repository: https://github.com/jegelstaff/formulize

Video tutorials for using Formulize (the full series is about three hours, but you can skip around between various videos at your leisure): http://formulize.org/formulize-workshop

Learn about our version control and continuous integration process: https://jegelstaff.github.io/formulize/developers/

---

### 8. Swift Support in WALA

Apple is a dominant player in the mobile space, and Swift is its new language for writing mobile apps. While Apple provides tooling based on LLVM, that is low-level machinery that is not readily usable by researchers working on program analysis at a higher level. Current research frameworks such as WALA and SOOT have little support for Swift, while, on the other hand, they provide extensive support for Android, even its latest versions. The result is a plethora of published tools for Android, e.g. Flowdroid, Scandroid, Stringoid, DroidInfer to name a few, and a relative dearth of tools for Apple platforms.
Given the popularity of Apple products and that wealth of published work for Android based on available infrastructure, we believe that lack suitable Swift infrastructure is a significant impediment. So support for Swift in a major platform like WALA would enable a wide range of new work.

Apple’s security model is significantly different from that of Android, for example; similarly Swift is rather different from popular languages on Android, especially at the type system level. It would be interesting to understand how these aspects affect program analysis, and analysis infrastructure is a prerequisite for such investigations.

There has been some ongoing work on Swift support since the WALA hack-a-thon held at  PLDI 2017 , where the hack-a-thon participants implemented some basic level of functionality for people to explore call WALA from within the Swift compiler.

#### Concrete project idea

Evaluate and extend Swift call graph construction in WALA for some open source Swift code, and create any needed special-purpose policies to avoid precision loss in the face of advanced Swift features.  

Mentors  

 * Karim Ali, University of Alberta
 * Julian Dolby, IBM T. J. Watson Research Center
 
#### Required skills
 * Good knowledge of compilers and/or some knowledge of the LLVM infrastructure
 * Knowledge of Swift is beneficial
 * C/C++ programming
 * Java programming
 * Knowledge about program analysis is a plus.

---

### 9. Safe Browsing and Tracker Prevention

#### Problem statement:

Current state-of-the art work on safe browsing and tracker prevention largely rely on heuristic `[1]` approaches or (semi) manually updated white/black lists `[2]`. When it comes to measuring the efficacy of privacy and tracking protection service, client-side performance is difficult to asses. Using web crawler technology to study the incidence and prevalence of tracker code also has limitations in terms of the portion of the web that can be seen. Current anti-tracking technologies attempt to block the execution of (primarily `[3]`) javascript code deemed to be providing tracking assets to third-party entities. Intervention in these cases can lead to unpredicted breakage in the functionality of websites. Furthermore, both client-side evaluation and crawler based assessment of potential fingerprinting attacks can not provide a known false negative rate when it terms of fingerprinting attacks that are undetected based on heuristic methods and blacklist-based approaches.

#### Project contribution:

We would like to gather a labeled dataset to guide development of (rule-based) classification of page elements in real time. The aim would be to prevent tracking code from executing while minimizing page breakage. The classifier should be evaluated such that it generalizes well to new pages without the need for a black-list/white-list paradigm.
The project will combine a small set client-side measurements for a group of opt-in users’, measured during unperturbed web browsing. The set of metrics to be collected in this context will be discussed during the September UCOSP sprint with the first full team deliverable being a finalized list of measurements to be delivered on or before October 18th. Measurement of features indicative of fingerprinting should be the primary focus with additional features relating to the user experience also considered; for example: page breakage, load-times, layout disruption, etc. Some starting points of projects active in this technology space are here:  [chameleon](https://github.com/ghostwords/chameleon), [panopticlick](https://gist.github.com/mlopatka/0932beb331d64836938018d42810af4a), [cliqz](https://github.com/cliqz-oss/privacy-bot). 

#### Design and Deliverables:

A web extension will be developed to perform data collection on an opt-in cohort of firefox users. Broad spectrum Javascript API calls to a variety of sources will be logged on a page-visit level. Information collected regarding api calls will be obfuscated on the client side using an [adaptation of the RAPPOR algorithm ](https://github.com/Alexrs95/rappor) before payload delivery. This will facilitate access to the raw data by UCOSP participants.

Collaboration on this project between Mozilla and openWPM maintainer [Steven Engelhardt](https://senglehardt.com) will allow us to combine this information with a broader view of such API calls by detecting their  occurrence in a  large corpus of crawl data. One team member will be tasked with interfacing the classifier trained on our client data with the openWPM platform.

In order to improve upon current methods for assessing anti-tracking performance, a criteria of “information leakage” will be developed and articulated in the context of reference statistics derived from the crawl data. This quantity will relate to the distinctiveness of a particular browser visit to a page in a feature space defined by the information accessible by the page.

The data derived from this two-prong collection will generate a semi-labeled dataset with which to train a classifier that does not rely on black-list/white-list resources. Assuming a sufficiently level of performance is achieved, such a classifier could be used to generate and update a black-list by periodic crawls or perform tracking-blocking in real time if deployed in a web extension. A reach goal of this project will be to investigate the feasibility of detecting and clocking first-party tracking efforts, which are a [growing concern](https://medium.com/firefox-context-graph/are-trackers-the-new-backbone-of-the-web-fb800435da15) as a small number of entities gain ever-larger presence on the web.

#### Modular components (student roles):

1. a) One team member will be tasked primarily with continuing work on [a web extension to log all javascript API calls](https://github.com/groovecoder/data-leak) executed during full scope of page interaction. Data collection may be extended to include page breakage and load time metrics.
   b) The payload of Javascript api calls at the page level must be obfuscated using to guard against domain/page profiling attacks by fingerprinting. Dave Zeber, will co-mentor a second team member focussed on evaluating the possibility of extending existing differential privacy algorithms to this use case.
 
2. Defining a metric of "information leakage" that occurs on a page visit will be a parallel task assigned to a third team member. This task is a bit more research focussed and relies heavily on current literature. There is substantial research already available on this topic and it is an active domain. The metric properties will be specified during the September UCOSP sprint to enable its usability as a component in the other objectives of this project. Example usage of this metric would be to help with risk assessment and further element-level actions. For pages with a very low leakage, no further action would be required. I.e. plain html pages not running javascript or setting cookies, should return a leakage value of 0.0. Pages collecting sufficient information to confidently and uniquely identify a single firefox visitor should return a leakage value of 1.0. Any value in between becomes part of the balancing act between blocking scripts (to decrease leakage) and preserving page functionality.

3. Data analytics and classifier implementation: In order to make use of the data collection efforts from both the client-collection and crawl portions, a feature selection procedure must be carried out. This will be performed by a fourth team member. This task may consider the additional context of information we can get from project  [Fathom](https://github.com/mozilla/fathom/blob/master/README.md). The features selected here will form the input space of a classifier that will assign a label of safe/not-safe to specific page elements. The efficacy of classification strategies will be evaluated against the information leakage metric described above. A substantial validation step will be required here to prototype and evaluate various approaches to this problem that are expected not only to prevent fingerprinting, but also (where possible) preserve page functionality.

#### Mentorship team:
Project lead: Martin Lopatka (Mozilla)

Differential Privacy expert: Dave Zeber (Mozilla)

TrackWare specialist: Luke Crouch (Mozilla)

OpenWPM and browser fingerprinting specialist: Steven Engelhardt (Princeton)

`[1]` [privacybadger](https://www.eff.org/privacybadger), [adblockplus](https://adblockplus.org)

`[2]` [disconnect.me](https://github.com/disconnectme/disconnect-tracking-protection), [ghostery](https://www.ghostery.com),  [uBlock](https://github.com/gorhill/uBlock/tree/master/assets)

`[3]` While most user information is exposed through JavaScript, there are some fingerprintable surfaces which can be compromised without the use of JavaScript. For example, HTTP headers could expose operating system type and version, and browser vendor and version. 