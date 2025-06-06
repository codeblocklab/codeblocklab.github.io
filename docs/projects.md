---
layout: page
title: Projects
---

{% for post in site.posts %}
  {% if post.project == 1 %}
  <div class="project-link">
    <a href="{{ post.url }}">{{ post.title }}</a>
  </div>
  {% endif %}
{% endfor %}

