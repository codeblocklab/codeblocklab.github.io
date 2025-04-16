---
layout: page
title: Skills
permalink: /skills/
---

{% assign skills = site.skills %}
{% for skill in skills %}
  <div class="skill">
    <h3>{{ skill.title }}</h3>
    <p>Tags: {{ skill.tags | join: ', ' }}</p>
    <p>{{ skill.content | markdownify }}</p>
  </div>
{% endfor %}
