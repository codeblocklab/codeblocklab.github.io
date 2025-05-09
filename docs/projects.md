---
layout: page
title: Projects
---

{% for post in site.posts %}
  {% if post.project == 1 %}
  <a href="{{ post.url }}">{{ post.title }}</a>
  {{ post.excerpt }}
  {% endif %}
{% endfor %}

