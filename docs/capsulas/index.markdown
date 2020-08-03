---
layout: default
title: Cápsulas
nav_order: 3
---

# Cápsulas

Contenidos asincrónicos.

<ul class="pages">
  {% for page in site.pages %}
  {% if page.categoria == "capsula" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>