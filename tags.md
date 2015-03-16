---
layout: page
title: Tags
permalink: /tags/
---
<h1>How to list your jekyll posts by tags</h1>

This code taken from <a href="http://www.jokecamp.com/blog/listing-jekyll-posts-by-tag">http://www.jokecamp.com/blog/listing-jekyll-posts-by-tag/</a>

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}

  <div class="tag">{{ t | downcase }}</div>

  <ul>
    {% for post in posts %}
      {% if post.tags contains t %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
        </li>
      {% endif %}
    {% endfor %}
  </ul>
{% endfor %}
