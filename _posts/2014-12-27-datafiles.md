---
layout: post
title:  "Introduction to datafiles"
tags: intro datafiles
---
Taken from <a href="http://jekyllrb.com/docs/datafiles/">http://jekyllrb.com/docs/datafiles/</a>

<ul>
{% for org_hash in site.data.orgs %}
{% assign org = org_hash[1] %}
  <li>
    <a href="https://github.com/{{ org.username }}">
      {{ org.name }}
    </a>
    ({{ org.members | size }} members)
  </li>
{% endfor %}
</ul>



