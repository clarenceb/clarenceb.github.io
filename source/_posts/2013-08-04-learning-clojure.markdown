---
layout: post
title: "Learning Clojure"
date: 2013-08-04 22:48
comments: true
categories: clojure programming 
---

The land of Clojure goodness
----------------------------

A couple of weeks ago I rolled off from my previous client and I joined an existing project at a new client.   My new project has already been active for about a year now.  The interesting thing from a technology point of view is that the core language used on this project is [Clojure](http://clojure.org/).   The prospect of learning and using a functional programming language like Clojure is very exciting for me as I spent the last several months on a project where the main language used was good old boring Java.

Most of my career I've been doing imperative-style programming, usually in the form of Object-Oriented programming.  Earlier this year I tried my hand at [Scala](http://www.scala-lang.org/) by following along in the excellent [Coursera](http://www.coursera.org/) course [Functional Programming Principles in Scala](https://www.coursera.org/course/progfun).  This course taught me a few of the fundamental Functional Programming concepts so I wasn't completely new going into Clojure.

What is Clojure?
----------------

Briefly, Clojure is a general purpose, functional, dynamic programming language which targets the Java Virtual Machine (JVM).    Clojure is a dialect of Lisp.  I remember learning Lisp when I was at University and I remember all the peculiar nested parentheses that confused me at times.  Luckily, Clojure makes some trade-offs in favour of wider adoption and accessibility to mainstream developers over being a pure Lisp clone.  This means that you'll see syntactic sugar and other data structures - not everything is a list.

Where did I start my learning?
------------------------------

Luckily, I had a couple of days before starting on my new project to get some exposure to Clojure.  I started with the awesome [Clojure Koans](http://clojurekoans.com/).  The Koans are mini exercises where you fix failing tests by writing code and you follow a learning path through the main parts of Clojure.  Next, I started looking at [4Clojure.com](http://www.4clojure.com/) where you solve progressively harder problems by filling in code snippets and submitting your solution - this is entirely web based so no extra tools are required though you should have some basic Clojure knowledge first.

How is going so far?
--------------------

I'm lucky in that I am in an awesome, supportive team that practices pair programming on all user stories.  This means that in the two short weeks that I have been on my project I have picked up a fair amount of Clojure and learnt some useful tips from experienced Clojure developers.  Clojure is mostly used in the backed services on my project and the front-end makes use of [AngularJS](http://angularjs.org/).  This means that I am dividing my time between learning Clojure and AngularJS (which is also new for me).

So far I'm finding Clojure to be a very powerful and productive language.  It reminds me of the "wow" moment I experienced when I first started learning [Ruby](http://www.ruby-lang.org/) after having spent a lot of time in C# and Java.  The first thing I noticed was how little code was required to implement a feature and without excessive ceremony and boilerplate code.

Tooling
-------

I am using Leiningen from the commandline for most build and testing tasks but using [IntelliJ IDEA](http://www.jetbrains.com/idea/) with the [La Clojure plugin](http://plugins.jetbrains.com/plugin?pluginId=4050) for code editing, navigation and refactoring.  IntelliJ was chosen by the team I joined so I am just sticking with that for now.  Another team using Clojure at my current client develops in [Emacs](http://www.jetbrains.com/idea/).  I'm keen to try out Emacs when I am a bit more confident with Clojure as I don't want to introduce too many new things at once!

What's next?
------------	

I'm currently going through the book [Programming Clojure (2nd edition)](http://pragprog.com/book/shcloj2/programming-clojure) by Stuart Halloway and Aaron Bedra to gain a bit more depth and breadth in Clojure.  However, I expect to get better at it through practice and pairing on a real production codebase (i.e. my client project described earlier).
