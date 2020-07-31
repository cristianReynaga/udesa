---
layout: default
title: tuto2
nav_order: 8
search_exclude: true
---

# Tutoriales 2 

<ul class="posts">
   {% for post in site.posts %}
      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ post.url }}">{{ post.title }}</a></li>
   {% endfor %}
</ul>