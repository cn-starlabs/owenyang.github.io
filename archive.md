---
layout: default
title: All Posts
permalink: /archive/
---

# Archive

{% for post in site.posts %}
  <div style="margin: 1em 0;">
    <a href="{{ post.url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%b %-d, %Y" }}</small>
  </div>
{% endfor %}
