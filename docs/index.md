---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Codeblock skills
---

This page is dedicated to present our technical skills, describe usecases and our past projects. Feel free to reach out to us in case of any further questions

#### Skills

{% for sk in site.skills %}
  <h2>
    <a href="{{ sk.url }}">
      {{ sk.name }} - {{ sk.title }}
    </a>
  </h2>
  <p>{{ sk.content | markdownify | truncate: 100 }}</p>
{% endfor %}
scokolwiek jeszcze cokolwiek 
