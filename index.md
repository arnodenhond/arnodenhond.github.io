---
layout: default
title: Blog
---

{% for post in site.posts %}
<div class="post-card">

  {% if post.cover_image %}
  <a href="{{ post.url | relative_url }}">
    <img src="{{ post.cover_image | relative_url }}" alt="{{ post.title }}">
  </a>
  {% endif %}

  <div class="post-info">
    <h2>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>

    <small>{{ post.date | date: "%B %d, %Y" }}</small>

    <p>{{ post.subtitle }}</p>
  </div>

</div>
{% endfor %}
