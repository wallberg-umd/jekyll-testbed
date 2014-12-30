---
layout: page
title: Environments
permalink: /env/
---
{% assign env = site.data.environment %}
<ul>
  {% for service in env.services %}
    <li>{{ service.title }}</li>
  {% endfor %}
</ul>
