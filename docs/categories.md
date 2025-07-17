---
layout: page-with-sidebar
title: Categories
---

{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
  <h3 id="{{ tag[0] | slugify }}">{{ tag[0] }}</h3>
  <ul>
    {% assign sorted_posts = tag[1] | sort: 'title' %}
    {% for post in sorted_posts %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}