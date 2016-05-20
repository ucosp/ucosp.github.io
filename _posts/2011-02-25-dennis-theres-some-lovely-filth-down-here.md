---
id: 2806
title: 'Dennis! There&#8217;s some lovely filth down here!'
date: 2011-02-25T10:28:19+00:00
author: Karen Reid
layout: post
guid: http://ucosp.ca/?p=2806
permalink: /2009-2010/uncategorized/2011/02/dennis-theres-some-lovely-filth-down-here/
categories:
  - Uncategorized
---
We are now well underway in our ReviewBoard projects, though, like everyone, its a challenge to balance both UCOSP and the rest of our courses/lives/commitments. In addition, for some of us it seems our progress is pretty slow for the moment as we are still trying to learn the languages & digging down to see all the nit & grit of ReviewBoard!

I&#8217;m currently working on the scalability testing for ReviewBoard & its quite an interesting process to say the least. Django uses what it calls BaseCommands that allow you to write scripts that will populate databases normally filled through your web interface. However, I found the documentation on these commands to be pretty sparse, and, I suppose, for good reason. Django uses Python like the King Arthur&#8217;s horse uses coconuts (Monty Python). So a lot of the Django documentation was about the various types of command classes and not about implementing the seemingly restricted Python code required to make it function.

Django has three types of `BaseCommand` subclasses that you are supposed to use instead of the `BaseCommand` class itself. The three types are: `AppCommand` (for invoking applications), `LabelCommand` (for passing any kind of arbitrary arguments called labels), and the `NoArgsCommand` (which, to quote Django docs, &#8216;takes no arguments on the command line&#8217;). It took me a while to realize that the `NoArgsCommand` subclass does not really mean &#8216;no arguments&#8217; (at least what I&#8217;d consider &#8216;no arguments&#8217;).

Using the `NoArgsCommand` subclass you are actually still able to utilize command-line arguments that are indicated with a &#8216;&#8211;&#8216;. Once you know this it is quite easy to create custom command line arguments by simply adding them to the option list. For instance:

`11 class Command(NoArgsCommand):<br />
...<br />
14     option_list = BaseCommand.option_list + (<br />
15         make_option('-u', '--users', type="int", default=None, dest='users',<br />
16             help='Specifies the number of users to add to the db'),<br />
...`

This lets you run your script with the `--users=10` argument & parses the values for you and even ensures that the argument provided is an integer. Very slick! The nice part of the `NoArgsCommand` subclass is that there are a lot more examples on the web than the other `Command` subclasses.

So with that accomplished I&#8217;m now getting into the murk & mire of our ReviewBoard code, trying to learn how the database commands are invoked. The woman digging in the dirt from Monty Python & the Holy Grail couldn&#8217;t have said it any better: _&#8220;Dennis! There&#8217;s some lovely filth down here!&#8221;_

-Steve Sutcliffe