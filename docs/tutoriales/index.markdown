---
layout: default
title: Tutoriales
nav_order: 4
has_children: true
has_toc: false
---

# Tutoriales 

## Premiere Pro

<ul class="pages">
  {% for page in site.pages %}
  {% if page.tutorial == "Premiere" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>

## After Effects 

<ul class="pages">
  {% for page in site.pages %}
  {% if page.tutorial == "After" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>

## Resolume Arena  

<ul class="pages">
  {% for page in site.pages %}
  {% if page.tutorial == "Resolume" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>

## Otras aplicaciones

<ul class="pages">
  {% for page in site.pages %}
  {% if page.tutorial == "Otras" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>