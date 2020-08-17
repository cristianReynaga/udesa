---
layout: default
title: Otras Aplicaciones
parent: Tutoriales
nav_order: 4
has_children: false
---

# Otras Aplicaciones

<ul class="pages">
  {% for page in site.pages %}
  {% if page.tutorial == "Otras" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>