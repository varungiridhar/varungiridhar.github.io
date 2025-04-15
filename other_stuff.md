---
layout: page
title: Other stuff
permalink: /other_stuff/
---

<!-- <h1>Posts</h1> -->
<ul class="post-list">
  {% for post in site.posts %}
    <a href="{{ post.url | relative_url }}" class="post-card-link">
      <li class="post-card">
        {% if post.featured_image %}
          <div class="post-card-image">
            <img src="{{ '/assets/' | append: post.featured_image | relative_url }}" 
                 alt="{{ post.featured_image_alt | default: 'Featured image' }}">
          </div>
        {% endif %}

        <h2>{{ post.title }}</h2>

        {% if post.subheading %}
          <p class="post-card-subheading">{{ post.subheading }}</p>
        {% endif %}

        <p class="post-meta">
          {{ post.date | date: "%b %-d, %Y" }}
        </p>
      </li>
    </a>
  {% endfor %}
</ul>