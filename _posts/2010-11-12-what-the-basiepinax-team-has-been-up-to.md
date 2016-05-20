---
id: 2787
title: What the Basie/Pinax team has been up to.
date: 2010-11-12T16:27:51+00:00
author: Andrew Louis
layout: post
guid: http://ucosp.ca/?p=2787
permalink: /fall2010/2010/11/what-the-basiepinax-team-has-been-up-to/
categories:
  - Fall 2010
---
_A guest post by team member Todd Ritchie._

The Basie/Pinax team has been working on a mailing list module for the next iteration of Basie. This module was designed with the intent of being able to decouple it from Basie and use it with any Pinax application. We started from scratch and during the code sprint we managed to get creation of mailing lists working, addition of subscribed e-mail lists, and walking of subscribed e-mails so that we can send messages.

We’ve been busy since then and have met on Wednesday mornings on the basie IRC channel. We have a team of four so voting doesn’t always work since there can be an even split. We’ve implemented a rotating position of dictator-for-the-week who has the final say on issues so we can proceed quickly. Recently we’ve decided to meet on Thursday evenings as well. Since the code sprint we have implemented receiving of mail with the help of a procmail script, better views for management of subscribers and mailing lists, verification of e-mail addresses, parsing and storing of incoming mail, and a first attempt at sending mail. Everyone has had the chance to move back and forth between different parts of the MVC model.

During the code sprint Kyle and Todd started with the database back end and the first template. Lance and Joel began with the mail parser. The pairs then swapped to Joel and Kyle working on the parser and Lance and Todd working on the subscription datamodel and management. Kyle integrated the mail receiver with our script and mangled strings for the parser, Todd and Lance have swapped who’s worked on views versus who’s working on templates and Joel has focused on the parser as well and sending mail.

The challenge we faced most recently is working out the best way to send mail. We have essentially three choices as outlined in our [mail sending ticket](https://bitbucket.org/basie/mailrelay/issue/19/create-send-methods-for-listmessage-and). The latest stable version of Pinax does provide an API for sending mail, but it does not allow you to add headers. The development version of Pinax has a new function that allows you to add your own headers. We could create our own mailer, but then we would have to maintain two mailers since the library we use for e-mail address verification relies on the Pinax mailer. Between these three choices we’ve decided to go with the latest development version of Pinax rather than do without essential mailing list headers or maintain or own mailer code.

Our next steps are to migrate to a newer version of the Pinax library so that we can modify headers while sending mail, to improve our existing list management templates, to write templates and views to read archived mail ([ticket #20](https://bitbucket.org/basie/mailrelay/issue/20/create-views-for-accessing-archived-email), [ticket #23](https://bitbucket.org/basie/mailrelay/issue/23/create-templates-for-accessing-archived)), and to polish what we’ve got.

We intend to enter a feature freeze after these features have been implemented and work on improving the installation process, create external documentation, make sure that our tests have adequate coverage, and make sure that our code conforms to the [Pinax style guide](http://pinaxproject.com/docs/dev/contributing.html#coding-style).