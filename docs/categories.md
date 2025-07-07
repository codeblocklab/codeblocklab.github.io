---
layout: page-with-sidebar
title: Categories
---

{% for tag in site.tags %}
  <div class="tag-section" id="{{ tag[0] | slugify }}">
    <h3>{{ tag[0] }}</h3>
    <ul>
      {% for post in tag[1] %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}


