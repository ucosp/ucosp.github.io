---
title: Projects (Sept 2018)
author: ucosp-steering
layout: default
---
### Overview

We have an excellent list of projects, and I'd like to thank all the project mentors for taking the time to work with our students.

### September 2018 

  1. **Review Board:**
  2. **UMPLE:**
  3. **Firefox Debugger**
  4. **Formulize**
  5. **Tracking Tecnologies on the Modern Web**

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
  
### 3. Firefox  debugger

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


### 4. Formulize

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

Students will have extensive exposure to PHP of course, and related web technologies. There are several priority areas of work at the moment, which students may participate in depending on aptitude and interest: the Selenium-based functional testing environment needs updating to fix failing tests; we would like to make it possible to copy/clone elements from one form to another so users don't need to recreate the same settings manually; we would like more automatic handling of creating database relationships between forms (one-to-one, one-to-many) and a better user interface for managing relationships.

Learn more about Formulize:

Download Formulize and docs: http://formulize.org/formulize-downloads

Browse the GitHub repository: https://github.com/jegelstaff/formulize

Video tutorials for using Formulize (the full series is about three hours, but you can skip around between various videos at your leisure): http://formulize.org/formulize-workshop

Learn about our version control and continuous integration process: https://jegelstaff.github.io/formulize/developers/


---

### 5. Safe Browsing and Tracker Prevention

Project​ ​keywords​: Data Mining, Tracking Protection, Machine Learning, Web Technologies.

#### Problem statement: 

Current work on the Mozilla Overscripted`[1]` corpus is aimed at developing a prototype method for online tracking interventions using large scale data analysis and Machine Learning. Current state-of-the art tracking protection methods largely rely on heuristic approaches or (semi) manually`[2]` updated white/black lists. When it comes to measuring the efficacy of such approaches, both the client-side experience and the actual efficacy at disrupting tracking is difficult to asses.
This project will continue to extend the exploratory analysis into the potential for real-time and element-wise tracker protection that can operate independent of a whitelist/blacklist paradigm by offline training of classification models that are pushed to the client so as to deliver tracking protection without compromising client privacy.

#### Project contribution: 

In the previous UCOSP cycle, students performed a large-scale data analysis of web page data, including javascript execution traces from over 1 million websites. While hyperlinking connectivity on this dataset can be assessed, a true representation of web traffic can not be inferred. The​ ​focal​ ​point​ ​of this​ ​project​ ​will​ ​be​ ​to​ ​perform​ ​an​ ​in-depth​ ​analysis​ ​of​ ​the​ ​crawl​ ​data​ ​in​ ​order​ ​to​ ​prepare​ ​a statistical​ ​measure​ ​of​ ​the​ ​data​ ​leakage​ ​incurred​ ​when​ ​a​ ​particular​ ​page​ ​is​ ​visited​. This information leakage criteria will inform a browser-loaded webextension to help users attain a general understanding of what Tracking Technologies are prevalent on today’s Web. Then we will use the combined view of the crawler data and telemetry form the webextension to evaluate various strategies for dynamic tracking protection models.
The project will use the crawl data already collected as a surrogate for actual user browsing data while the project team, in collaboration with other Mozilla engineers, prototype an element-level javascript blocking approach. This work will later be used to collect a small set of client-side measurements for a group of opt-in users. Measurement of the quantitative privacy loss incurred as a result of javascript elements indicative of fingerprinting should be the primary focus of the project.

#### Project Context:

Preliminary work on browser fingerprinting has been done by the EFF utilizing a worst-case assumption of data collection`[3]`; this will be both a starting point and a baseline for evaluating tracking protection performance. While most user information is exposed through JavaScript, there are some fingerprintable surfaces which can be compromised without the use of JavaScript. For example, HTTP headers could expose operating system type and version, and browser vendor and version.



### Mentorship team:

Sarah Bird, Daid Zeber, Victor Ng, Luke Crouch, Martin Lopatka (Mozilla)
`[1]` https://github.com/mozilla/Overscripted-Data-Analysis-Challenge

`[2]` https://www.eff.org/privacybadger 

`[3]`https://www.eff.org/deeplinks/2017/11/panopticlick-30 

