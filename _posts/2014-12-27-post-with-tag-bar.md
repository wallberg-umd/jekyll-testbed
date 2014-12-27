---
layout: post
title:  "This post has tag bar (with foo)"
tags: foo bar
---
This is a generated list of tags on this post:

<ul>
 {% for tag in page.tags %}
   <li>{{ tag }}</li>
 {% endfor %}
</ul>

