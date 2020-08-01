---
layout: default
title: Clases
nav_order: 2
---

# Clases

Contenidos y slides de los módulos. 
{: .fs-6 .fw-300 }

## Clases sincrónicas

<ul class="pages">
  {% for page in site.pages %}
  {% if page.categoria == "clases" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>

## Cápsulas asincrónicas

<ul class="pages">
  {% for page in site.pages %}
  {% if page.categoria == "capsula" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>