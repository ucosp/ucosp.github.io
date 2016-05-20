---
id: 2994
title: How to Generate UML Diagram of Models in Django Project
date: 2016-01-12T11:05:29+00:00
author: ucosp-steering
layout: post
guid: http://ucosp.ca/?p=2994
permalink: /2009-2010/uncategorized/2016/01/how-to-generate-uml-diagram-of-models-in-django-project/
categories:
  - Uncategorized
---
(An experience report from Yorie Nakayama)

If you are developing with python on Django, or on any frameworks that
  
employ the MVC (Model-View-Controller) paradigm, you might come across
  
whether there is a way to easily visualize all the models and their
  
dependency relationships in your application as a diagram. Models are
  
central to most applications using MVC, and being able to glance at the
  
structure of models and their relationships to each other greatly helps
  
any developer beginning to hack on the codebase.

When I worked with Reviewboard, a Django-based web app for doing code
  
reviews, for my UCOSP, one of the first things I did was to generate a
  
UML diagram of the models in the project using an extension package for
  
Django called django-extensions. The diagram would let the students, who
  
are new to the project, to see the overall picture of the models, and
  
also let the mentors easily explain how some models are related to each
  
other.

This post will provide a step-by-step instruction on generating a UML
  
diagram of a Django application using django-extensions. Similar tools
  
also exist for other MVC frameworks, such as railroady gem for Ruby on
  
Rails, or phuml for PHP (not limited to CodeIgniter).

1. Install Dependencies.
  
For python, you need to install either pydot or pygraphviz as a python
  
interface of the graph visualization library called graphviz. Either
  
will be fine as far as django-extensions is concerned. I went with pydot
  
because I had a trouble installing pygraphviz. If you choose to go with
  
pygraphviz, you can ignore this step and resume from step 2 after
  
installing pygraphviz.

pip install pyparsing==1.5.7
  
pip install graphviz
  
pip install pydot

The version is specified on pyparsing installation because pydot is not
  
compatible with newer (>=2.x.x) versions of pyparsing. I recommend that
  
graphviz is installed before pydot to avoid an issue where pydot is not
  
able to find graphviz executable. A similar installation issue may also
  
occur with pygraphviz.

2. Install django-extensions.
  
Django-extensions provides various tools that could help development of
  
Django applications such as enhanced shell, or UML diagram generation.

pip install django-extensions

3. Enable django-extensions in your project.
  
Under your Django project directory, open the file setting.py with a
  
text editor. Within the settings, you should find a python list called
  
INSTALLED_APPS.
  
Append &#8216;django_extensions&#8217; to the list and save. Then you can use the
  
functionalities that django-extensions provides.

4. Generate the UML diagram.
  
On a command shell, go to the Django project directory, and execute the
  
following command to generate your diagram of all models in the project.

python manage.py graph\_models -a -o myapp\_models.png

The -a flag specifies to include all apps listed in INSTALLED_APPS for
  
diagram generation. The output path is relative to the project root
  
directory.
  
If you decide that your project does not need django-extensions, you can
  
simply remove &#8216;django\_extensions&#8217; from INSTALLED\_APPS in settings.py.

With a UML diagram for your models, you can easily see the overall
  
picture of the data organization in your application. Hopefully this
  
diagram could help a new member on a Django project to find where to
  
start with the development.

&#8212; Yorie Nakayama