---
layout: page
title: Work
permalink: /work/
---
A work in progress...
<ul>
  {% for post in site.categories.work %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>