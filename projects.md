---
title: Projects (January 2017)
author: ucosp-steering
layout: default
---
### Overview

We have an excellent list of projects, and I'd like to thank all the project mentors for taking the time to work with our students.

### January 2018 (In progress)

  1. **Review Board:**
  2. **UMPLE:**
  3. **Firefox Code Coverage**
  4. **Firefox React Debugger**
  5. **Firefox Developer Tools - Inspector inline editor wigets**
  6. **Formulize**
  7. **WALA Program Analysis for Swift**
  8. **Safe Browsing and Tracker Prevention**

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

### 3. Firefox CodeCoverage 

#### Context

Firefox is a huge project, consisting of around 20K source files and 3M lines of code (if you only consider the Linux part!), supporting officially four operating systems, and being written in multiple programming languages (C/C++/JavaScript/Rust). We have around 200 commits landing per day in the mozilla-central repository, with developers committing even more often to the try repository. Usually, code coverage analysis is performed on a single language on small/medium size projects. Therefore, collecting code coverage information for such a project is not a small task. But code coverage can be used for many purposes, and at Mozilla, we have great ideas of how to use it to better the quality of each version of Firefox and to make a developers job easier by providing more data and easier testing.

#### Goals

Mozilla has two long term goals for CodeCoverage.

#### Is new source code covered by existing tests?

For a given changeset, what new lines of source code are covered? If new lines are not covered, are they important?  Should we write more tests?

The Release Management team will use this to spot trends of increased or decreased coverage by module (top level directory in the source tree) and work with module owners/managers to understand risks and plan future work. They will also use this data to look at coverage changes in soon-to-land, or landed, patches. 

*This interface has gone through a single iteration of feedback, and now needs polish: [See milestone](https://github.com/mozilla/firefox-code-coverage-frontend/milestone/4)*


#### Per-test Coverage

For any file, for any revision, show what tests cover that file.

* Developers can determine what tests should be run based given the files they have changed.
* Component owners can inspect how tests overlap coverage, which will help determine if tests are redundant.

[This interface is is going through review now](https://github.com/mozilla/firefox-code-coverage-frontend/pull/76) and will soon be ready for a round of feedback from users within Mozilla. This feedback will undoubtedly generate a list of fixes and features to work on. 

*Coverage is not collected at a per-test level yet, but we hope to have some initial data after January*


#### Deliverable

UCOSP students will make enhancements to the UI, as listed by the GitHub Issues. This will allow the student to acquire working experience in HTML, JSX, React and Javascript.


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

### Firefox Developer Tools - Inspector

[Firefox Developer Tools](https://developer.mozilla.org/en-US/docs/Tools) (DevTools) allow developers to inspect and debug their web applications. The DevTools are built using web technology such as HTML, CSS and JavaScript utilizing the latest web libraries such as React and Redux.

In the Inspector, we will be working on a number of tools related to various CSS properties, Layout and Font inspection. Some examples of these new tools and features that previous students have worked on included:

* CSS Grid Inspector
* Box Model Layout panel improvements
* CSS Variables Inspection

To read about some of the accomplishments from previous UCOSP students, visit https://hacks.mozilla.org/2017/06/new-css-grid-layout-panel-in-firefox-nightly/.

For the Inspector, we want to continue to working on better CSS Layout tooling such as CSS Grids and Flexbox inspector. In addition, we are aiming to implement more visual editors that will help developers and designers with debugging and editing complex CSS properties visually. Since CSS is very declarative by nature, we can provide tools that are commonly found in digital design tools, such as Adobe Photoshop and Illustrator, and Sketch, in order to bridge the learning gap of new developers and designers learning CSS. This would allow them to edit various CSS properties such as box-shadow, clip-path, gradient, filters, etc without knowing what the properties are.

Our goal is to help developers and designers come into the Inspector and be able to easily edit and learn HTML and CSS, and make changes to their web pages and eventually provide better authoring tools to help them also extract these changes.


---

### 6. Formulize

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

The newer parts of the codebase employ some object orientation. Older parts remain largely procedural. The codebase is maintained on GitHub. Over the years, Formulize has developed a specific process for managing code, tests and documentation all through our GitHub repository. Our the tests are run automatically by a continuous integration system, based on Travis-CI and Sauce Labs. Students will have exposure to this process as part of contributing to the Formulize project.

#### What will students learn?

Students will have extensive exposure to PHP of course, and related web technologies. This term, we will be focusing on creating a web services API that will allow the cross-site integration of Formulize to operate via http requests, not just through server-side includes as it does now. Students who are interested in web technologies, particularly web services, are strongly encouraged to join the project this term.

Learn more about Formulize:

Download Formulize and docs: http://formulize.org/formulize-downloads

Browse the GitHub repository: https://github.com/jegelstaff/formulize

Video tutorials for using Formulize (the full series is about three hours, but you can skip around between various videos at your leisure): http://formulize.org/formulize-workshop

Learn about our version control and continuous integration process: https://jegelstaff.github.io/formulize/developers/

---

### 7. Swift Support in WALA

Apple is a dominant player in the mobile space, and Swift is its new language for writing mobile apps. The LLVM-based tooling that Apple provides is low-level machinery that is not readily usable by researchers working on program analysis at a higher level. Current research frameworks such as WALA and SOOT have little support for Swift, while, on the other hand, they provide extensive support for even the latest versions of Android. The result is a plethora of published tools for Android, e.g. Flowdroid, Scandroid, Stringoid, DroidInfer to name a few, and a relative dearth of tools for Apple platforms. 

Given the popularity of Apple products and a wealth of published work for Android based on available infrastructure, we believe that a lack of suitable Swift infrastructure is a significant impediment. Therefore, support for Swift in a major platform like WALA would enable a wide range of new work. For example, Apple's security model is significantly different from that of Android; similarly, Swift is rather different from popular languages on Android, especially at the type system level. It would be interesting to understand how these aspects affect program analysis, and analysis infrastructure is a prerequisite for such investigations.

There has been some ongoing work on Swift support since the WALA hack-a-thon held at PLDI 2017, where participants implemented some basic level of functionality for people to explore call WALA from within the Swift compiler. During UCOSP Fall 2017, the team was able to add WALA support for some Swift features including Integer Literals, String Literals, and Boolean Short-Circuit Evaluation.

#### Concrete Project Ideas
1. Working primarily in the Swift compiler (C++, LLVM), evaluate and extend Swift call graph construction in WALA (Java, through JNI) for open-source Swift code, and create special-purpose policies to avoid precision loss in advanced language features
2. Write test cases which exercise high- and low-level language features in order to evaluate accuracy and coverage of the Swift-WALA project

#### Mentors
Karim Ali, University of Alberta
Julian Dolby, IBM T. J. Watson Research Center

#### Required Skills
 * Good knowledge of compiler theory and components
 * Advanced C/C++ programming experience
 * Comfortable working in a purely command-line Unix environment
 * Software engineering knowledge (e.g. working with and implementing various design patterns)

#### Assets
 * Knowledge of Swift programming language
 * Some knowledge of the LLVM infrastructure
 * Experience working with Git in a distributed team environment
 * Java programming experience
 * Program analysis knowledge/experience
 * macOS machine with > 8GB RAM (can be compiled on Ubuntu as well, but is more difficult)

#### Languages/Technologies: experience in any or all of these is an asset
C++, Java, Swift, JNI, LLVM, Swift Compiler, WALA, Static Analysis, Mac/Ubuntu CLI, Xcode, clang, Maven, Ninja, CMake

---

### 8. Safe Browsing and Tracker Prevention

#### Problem statement: 

Current work on safe browsing and tracker prevention largely rely on heuristic `[1]` approaches or (semi) manually updated
white/black lists `[2]`. When it comes to measuring the efficacy of privacy and tracking protection service, client-side performance is difficult
to asses. Current anti-tracking technologies attempt to block the execution of (primarily `[3]`) javascript code deemed to be providing tracking
assets to third-party entities. This project will perform largely exploratory analysis into the potential for real-time and element-wise
tracker protection.

#### Project contribution: 

In the previous UCOSP cycle, students performed a large-scale data collection of web page data, including javascript
execution traces from just under 1 million websites. While hyperlinking connectivity on this dataset can be assessed, a true representation
of web traffic can not be inferred. The focal point of this project will be to perform an in-depth analysis of the crawl data in order to
prepare a statistical measure of the data leakage incurred when a particular page is visited . This information leakage criteria will inform
a browser-loaded webextension to help users attain a general understanding of what Safe Browsing means on today’s web.

The project will use the crawl data already collected as a surrogate for actual user browsing data while the project team, in collaboration
with other Mozilla engineers, prototype an element-level javascript blocking approach. This work will later be used to collect a small set of
client-side measurements for a group of opt-in users. Measurement of the quantitative privacy loss incurred as a result of javascript
elements indicative of fingerprinting should be the primary focus of the project. Some starting points of projects active in this technology
space are here: [chameleon](https://github.com/ghostwords/chameleon), [panopticlick](https://www.eff.org/deeplinks/2017/11/panopticlick-30), [cliqz](https://github.com/cliqz-oss/privacy-bot).

#### Design and Deliverables:

Broad spectrum Javascript API calls have been collected for a set of crawled websites. A future aim shall be to use the findings from this
large data set to evaluate the actual experience of users’ experiences online. In order Information collected regarding api calls will be
obfuscated on the client side using an adaptation of the RAPPOR algorithm before payload delivery. This will facilitate access to the raw
data by UCOSP participants. 

In order to improve upon current methods for assessing anti-tracking performance, a criteria of “information
leakage” will be developed and articulated in the context of reference statistics derived from the crawl data. This quantity will relate to
the distinctiveness of a particular browser visit to a page in a feature space defined by the information accessible by the page. Preliminary
work on browser fingerprinting has been done by the EFF utilizing a worst-case assumption of data collection; the work performed in this
project will compliment that research by providing a realistic model of attempted collection behaviour exhibited by websites in the wild.

#### Modular components (student roles):

1. Defining a metric of "information leakage" that occurs on a page visit will be a central task for all team members. One team member will
focus on the implementation of this metric in the context of team discussion and extensive review of current literature. There is substantial
research already available on this topic and it is an active domain. The metric properties will be specified during the January UCOSP sprint
to enable its usability as a component in the other objectives of this project. Example of the desired usage of this metric would be to help
with risk assessment and further element-level actions. For pages with a very low leakage, no further action would be required. I.e. plain
html pages not running javascript or setting cookies, should return a leakage value of 0.0. Pages collecting sufficient information to
confidently and uniquely identify a single firefox visitor should return a leakage value of 1.0. Any value in between becomes part of the
balancing act between blocking scripts (to decrease leakage) and preserving page functionality.

2. Visualization -- A key component to tracking protection is raising awareness of the mechanisms and severity of tracking. This may help
users to change their online behaviour through the use of tools that help protect against tracking. The data analysis of the crawl data
should for the basis of a sub-task related to visualizing privacy loss as a result of online tracking.

#### Prerequisite skills:

All students should be proficient in either python or javascript. Interaction with amazon’s s3 storage platform will be mandatory for data
access. Quantitative statistical analysis will play a critical role in the datamining component of the project.


### Mentorship team:

Project lead: Martin Lopatka (Mozilla)

Differential Privacy expert: Dave Zeber (Mozilla)

TrackWare specialist: Luke Crouch (Mozilla)


`[1]` [privacybadger](https://www.eff.org/privacybadger), [adblockplus](https://adblockplus.org)

`[2]` [disconnect.me](https://github.com/disconnectme/disconnect-tracking-protection), [ghostery](https://www.ghostery.com),  [uBlock](https://github.com/gorhill/uBlock/tree/master/assets)

`[3]` While most user information is exposed through JavaScript, there are some fingerprintable surfaces which can be compromised without the use of JavaScript. For example, HTTP headers could expose operating system type and version, and browser vendor and version. 

---

### 9. Filtering system for the Automated Benchmark Management (ABM) web application.


### Automated Benchmark Management (ABM)

A common way of testing software or research prototypes is to use well-known benchmark suites such as the DaCapo suite [1] for example. However, such large benchmarks are hard to create and to maintain, and this work is often done by hand. Moreover, benchmark suites currently only exist to test for specific properties, and are not necessarily adapted to the needs of the tested software. The Automated Benchmark Management (ABM) methodology [2] has been created to address the shortcomings of current benchmark suites. It aims at automatizing the process of benchmark creation and maintenance, and makes it fully customizable to the user, so that they can create benchmark suites adapted to their use. We are currently building a website [3] to implement the ABM methodology. The current implementation crawls GitHub for open-source, real-world projects. It allows users to filter out unsuitable projects using the Hermes project, which analyzes projects and collects various metrics [4], and create and update collections from the remaining projects.

#### Your work

After the initial search, users can filter out unsuitable projects, using sets of pre-defined filters. Your work will be to re-design and implement the user interface for the filtering module, and to improve its usability. At the end of this project, users should be able to easily select the set of projects they need with respect to the filters they select.

Your work will mainly focus on frontend programming in AngularJS. Interactions with the backend are handled in Java. ABM is managed through multiple branches on a git repository, and is updated using the Jenkins continuous integration system. 

#### Detailed tasks

1. Define the interactions between ABM and Hermes, and determine the requirements that Hermes should meet to implement the filtering module for ABM. Communicate the requirements for the filter modules to the Hermes team.
2. Design and implement the interface that shows the user the filtering options/results for a given collection of projects.
3. Close the loop to allow the user to filter projects using the new interface.
4. Implement secondary functionalities, such as caching Hermes results, or undo options in case the user mistakenly removes a project or runs the wrong filter(s).

#### Required skills: 

- Good understanding of Javascript. 
- Knowledge of relational database systems.
- Knowledge of software design and efficient programming. 
- Prior knowledge of AngularJS and web application development is a plus.

#### Learning outcomes:

- Frontend programming with AngularJS.
- Collaborative software development with git and Jenkins.

#### Mentors:
Karim Ali, University of Alberta

Lisa Nguyen, Fraunhofer IEM

Ben Hermann, Paderborn University

### References: 
[1]  Stephen M. Blackburn, et al. 2006. The DaCapo benchmarks: java benchmarking development and analysis. In Proceedings of the 21st annual ACM SIGPLAN conference on Object-oriented programming systems, languages, and applications (OOPSLA '06). ACM, New York, NY, USA, 169-190. DOI = http://dx.doi.org/10.1145/1167473.1167488

[2] Lisa Nguyen Quang Do, Michael Eichberg, and Eric Bodden. 2016. Toward an automated benchmark management system. In Proceedings of the 5th ACM SIGPLAN International Workshop on State Of the Art in Program Analysis (SOAP 2016). ACM, New York, NY, USA, 13-17. DOI: http://dx.doi.org/10.1145/2931021.2931023

[3] ABM: http://abm.cs.upb.de/abm/index.html#/ 

[4] Michael Reif, Michael Eichberg, Ben Hermann, and Mira Mezini. 2017. Hermes: assessment and creation of effective test corpora. In Proceedings of the 6th ACM SIGPLAN International Workshop on State Of the Art in Program Analysis (SOAP 2017). ACM, New York, NY, USA, 43-48. DOI: https://doi.org/10.1145/3088515.3088523 
