---
layout: post
title:  "Using Jekyll to serve a static JSON database"
tags: jekyll datafiles json database
---

I've added to this Jekyll site an example static database backed by a JSON
datafiles.  The database has two primary datasets, a set of
services and a set of servers with links between them.  See
[_data/environment.json](https://github.com/wallberg-umd/wallberg-umd.github.io/blob/master/_data/environment.json)
for the JSON database structure.

The pages which serve this content are [Services](/services/) and
[Servers](/servers/), which are created using the Jekyll markdown
pages
[services.md](https://github.com/wallberg-umd/wallberg-umd.github.io/blob/master/services.md)
and
[servers.md](https://github.com/wallberg-umd/wallberg-umd.github.io/blob/master/servers.md)
respectively.

See [Jekyll-DB](http://labs.panchadsaram.com/jekyll-db/) for a
different implementation which adds more client side dynamism.


