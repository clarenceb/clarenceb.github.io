---
layout: post
title: "Viewing Git History in Summary Form"
date: 2012-09-04 12:00
comments: true
categories: git tips scm
---
I use this one all the time for getting a nice summary of git commits:
```
git log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short
```
Here's what the output looks like (used on the Homebrew git repo):
```
* d66c9f3 2011-03-16 | Boost version bump to 1.46.1 [Clint Shryock]
* 43019ac 2011-03-16 | Update JRuby to 1.6.0. [Aku Kotkavuo]
* 8ffc126 2011-03-16 | Erlang R14B02 [Yurii Rashkovskii]
* 24f4ad5 2011-03-16 | Gearman 0.18 [Clint Shryock]
* ec6521e 2011-03-15 | Fix keg-only, non-system dupes [Adam Vandenberg]
* fa2f638 2011-03-15 | Document keg-only system duplicates. [Adam Vandenberg]
* 3338b14 2011-03-15 | install - change keg-only warning [Adam Vandenberg]
* 9eb7c19 2011-03-15 | keg-only: provide more info about system dupes [Adam Vandenberg]
* d600846 2011-03-15 | scantailor: add libtiff dependency [Adam Vandenberg]
* 309ae6b 2011-03-15 | keg - use proper inheritance style [Adam Vandenberg]
* 3b25f34 2011-03-15 | Add new fontforge git repo as HEAD [codingisacopingstrategy]
* ac95e5c 2011-03-15 | New formula: mpg321 [Luca Spiller]
* 48c0ab0 2011-03-15 | Fix homepage audit warnings [Adam Vandenberg]
```
The output will also show any tags and visually show branches and merges.

You can then add it to your git config as an alias:
```
[alias]
  hist = log --pretty=format:\"%h %ad | %s%d [%an]\" --graph --date=short
```
And use it like so:
```
git hist
```
I got this tip from the following git tutorial site: [http://gitimmersion.com](http://gitimmersion.com/)
