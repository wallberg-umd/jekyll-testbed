---
layout: page
title: Services
permalink: /services/
---
{% assign env = site.data.environment %}

{% for service in env.services %}
  <a id="{{service.key}}"/>
  <h2>{{ service.title }}</h2>
  <ul>
    <li>Server: <a href="/servers/#{{ service.server }}">{{ service.server }}</a></li>
    <li>Aliases: {% for alias in service.aliases %} "{{ alias }}" {% endfor %} </li>
  </ul>
{% endfor %}
