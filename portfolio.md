---
layout: default
title: Portfolio
---

{% for project in site.projects %}
<div class="post-card">

  {% if project.cover_image %}
  <a href="{{ project.url | relative_url }}">
    <img src="{{ project.cover_image | relative_url }}" alt="{{ project.title }}">
  </a>
  {% endif %}

  <div class="post-info">
    <h2>
      <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
    </h2>

    <small>{{ project.platforms" }}</small>
    <br>
    <small>{{ project.technologies" }}</small>
    <br>
    <img src="https://playbadges.pavi2410.com/badge/downloads?id={{ project.packagename }}"/>

    <p>{{ project.description }}</p>
  </div>

</div>
{% endfor %}
