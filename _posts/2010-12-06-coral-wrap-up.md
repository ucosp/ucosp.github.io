---
id: 2789
title: CoRAL project wrapping up for the semester
date: 2010-12-06T20:38:00+00:00
author: Andrew Louis
layout: post
guid: http://ucosp.ca/?p=2789
permalink: /fall2010/2010/12/coral-wrap-up/
categories:
  - Fall 2010
---
_A guest post by the CoRAL team._

Since this project was conceptualized and named in early October, we have made great strides in designing a user and application programming interface for visualizing activity on [CoRAL (Collaborative Review Analysis of Literature)](http://hypatia.cs.ualberta.ca/ucospf10/wiki/index.php/Main_Page) and to be used in tandem with the [Fab4Browser](http://code.google.com/p/fab4browser/). CoRAL/Fab4 is an academic publication browser that allows users to comment, discuss and annotate academic papers. It was designed to facilitate discussion and development of ideas and encourage collaboration and sharing of viewpoints between different experts of the scientific community. CoRAL (Collaborative Review Analysis of Literature) is a web tool to visualize these networks, gauging the activity and impact of a paper on CoRAL users, and measuring the usage data of specific users.

UCOSP students designed and implemented visualizations that could be used to analyze the popularity of a paper, highlight discussions about the paper, and display networks arising from these conversations. Furthermore, visualizations were implemented to measure a user’s activity on CoRAL, papers read, and papers annotated. To complete the project, we used a PHP logic tier to interact with the DB2 database, and several JavaScript frameworks to implement the interactive visualization widgets. Students were able to independently develop the back-end logic and the separate widgets, and collaboratively piece together their work into a single interactive web application. Students simultaneously learnt the practical use of PHP and JavaScript, visualization, and techniques in code communication and collaboration.

The final product is a web tool that allows users to search for papers or other users on CoRAL and view information about the papers or users found. In the paper view, users are able to filter comments by the comment authors, and view on a timeline both when the paper was viewed and when comments were made. Furthermore, users can view the activity and popularity of users and comments based on comment ratings; user popularity and activity are visualized by their color and size on the network view. The person view displays both user activity and comments made on a timeline, and also displays a user’s interactivity with other users on a network graph. Furthermore, a summary of the user’s activity regarding papers read and comments made is displayed. The modular widgets can be adapted for use in other projects or pages involving CoRAL, or extended to display more complex analyses.

In just a few months, we have successfully created a flexible tool to visualize usage information about CoRAL. In addition to measuring how CoRAL is used, information about papers and users is particularly valuable in realizing how certain scientific social networks are formed and whether certain ideas or people are influential or controversial. More importantly, it can be used to track the evolution of ideas or pieces of writing as they become more refined and possibly eventually publishable. We are currently in the process of refining the application, and documenting it with the hopes that it may be further developed in the future!