---
layout: default
title: Resolume Arena
has_children: false
nav_exclude: true
nav_order: 3
parent: Tutoriales
has_toc: false
---

## Resolume Arena

<ul class="pages">
  {% for page in site.pages %}
  {% if page.tutorial == "Resolume" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>