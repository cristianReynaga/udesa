---
layout: default
title: After Effects
parent: Tutoriales
nav_order: 2
has_children: false
---

# After Effects

<ul class="pages">
  {% for page in site.pages %}
  {% if page.tutorial == "After" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>