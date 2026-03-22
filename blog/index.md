---
layout: archive
title: Статьи о машинной вышивке
permalink: /blog/ 
entries_layout: grid
author_profile: false
---

{% for post in site.posts %}

<div style="display:flex; gap:15px; margin-bottom:25px; align-items:center;">

  {% if post.image %}
  <img src="{{ post.image }}" style="width:120px; height:120px; object-fit:cover;">
  {% endif %}

  <div>

  <h3 style="margin:0;">
  <a href="{{ post.url }}">{{ post.title }}</a>
  </h3>

  <p style="margin:5px 0;">
  {{ post.content | strip_html | truncate: 80 }}
  </p>

  </div>

</div>

{% endfor %}