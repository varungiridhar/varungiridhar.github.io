---
layout: page
title: Work
permalink: /work/
---

<ul>
  {% for post in site.categories.work %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>