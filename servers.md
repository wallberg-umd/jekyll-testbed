---
layout: page
title: Servers
permalink: /servers/
---
{% assign env = site.data.environment %}

{% for server in env.servers %}
  <a id="{{server.key}}"/>
  <h2>{{ server.key }}</h2>
  <ul>
    <li>IPs:
	  <ul> {% for ip in server.ip %} <li>{{ ip }}</li> {% endfor %}</ul>
	</li>
	<li>Services:
	  <ul>
	    {% for service in env.services %}
	      {% if service.server == server.key %}
	    	  <li><a href="/services/#{{service.key}}">{{ service.title}}</a></li>
	      {% endif %}
	    {% endfor %}
	  </ul>
	</li>
  </ul>
{% endfor %}
