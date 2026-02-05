---
layout: default
title: Blog
permalink: /blog/
---

## Research Logs

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url }})**  
  <small>{{ post.date | date: "%d %B %Y" }}</small>
{% endfor %}
