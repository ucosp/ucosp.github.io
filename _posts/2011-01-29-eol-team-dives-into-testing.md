---
id: 2796
title: EOL team dives into testing
date: 2011-01-29T09:24:02+00:00
author: Karen Reid
layout: post
guid: http://ucosp.ca/?p=2796
permalink: /2009-2010/uncategorized/2011/01/eol-team-dives-into-testing/
categories:
  - Uncategorized
---
So we&#8217;re the Encyclopedia of Life (EOL) team: Josh (University of
  
Toronto), Jonathan (Ottawa University), Feng (York University), Tyler
  
and Will (both at Laurentian University) and our mentor is Dmitry
  
Mozzherin who is a programmer at Encyclopedia of Life.

Our project is to develop a general testing framework for the EOL
  
website &#8211; a site that is attempting to catalog every species on the
  
planet &#8211; with the intent that this framework be general enough to use
  
for any given website. We&#8217;re using a stack of technologies to
  
implement this goal:

Cucumber (http://cukes.info) is a behaviour driven development testing
  
framework developed in Ruby. It allows a programmer to describe what a
  
particular feature is intended to perform in plain English, and given
  
a set of underlying &#8216;step definitions&#8217; defined in Ruby, a test is
  
performed based on the plain English.

Selenium (http://seleniumhq.org/) is an automated way to control a web
  
browser and ensure that the behaviour of a website is correct.

Capybara (https://github.com/jnicklas/capybara) is a Ruby based driver
  
for the new version of Selenium. Our goal is to integrate Cucumber and
  
Capybara in such a way that automated tests can be performed using the
  
plain English descriptions mentioned above.

The potential benefits to combining these technologies are huge. Using
  
this software stack it should be possible to create an automated
  
testing framework that can be implemented in plain English and in a
  
generic way so that it can be used to test any website. The most
  
intriguing part of this whole project is that it is being started from
  
scratch. One of the administrators of the program noted that it was
  
almost unheard of for this to happen for Capstone projects but this
  
project seemed like a natural evolution from the current EOL testing
  
framework fit well with EOL&#8217;s goals.

Our time at the code sprint was spent for the most part getting
  
acquainted with Git, Ruby and the above technologies. Once we got
  
everything working in harmony we spent some time putting together some
  
initial tests which we&#8217;ll be able to use as templates for the bulk of
  
the work ahead us. The last day of the code sprint was spent dividing
  
up the work using the GitHub issue tracker which looks like it will be
  
an efficient way of distributing labour.

You can have a peek at our GitHub repository here:
  
(https://github.com/EncyclopediaOfLife/cukestone/)

Josh Zucker