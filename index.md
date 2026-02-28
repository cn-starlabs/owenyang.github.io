---
layout: default
title: Home
---

# Owen's Daily Notes

Welcome to my little corner of the internet.  

## Latest Posts

{% for post in site.posts limit: 10 %}
<div style="margin: 1.5em 0; padding: 1em; border-left: 4px solid #007acc; background: #f8f9fa;">
  <h3 style="margin: 0;">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h3>
  <small>{{ post.date | date: "%B %-d, %Y" }} • {{ post.reading_time | default: '2 min' }} read</small>
  <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
</div>
{% endfor %}

[See all posts →](/archive)   <!-- optional, create archive.md later if you want -->
