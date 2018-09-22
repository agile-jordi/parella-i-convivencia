---
layout: page
title: Som Parella
excerpt: "Som parella és un treball de reflexió i aprofundiment sobre la vostra parella, la relació entre vosaltres dos i amb tot allò que us envolta."
search_omit: true
---

## Temes

<ul class="post-list">
{% for post in site.categories.somparella reversed %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} {% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

