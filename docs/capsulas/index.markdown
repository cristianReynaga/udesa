---
layout: default
title: Cápsulas
nav_order: 3
---

# Cápsulas

Las cápsulas son contenidos asincrónicos, es decir, no forman parte del contenido de las clases, pero complementan y facilitan la profundización técnica y/o conceptual de herramientas o habilidades.

El tiempo que lleva las cápsulas es variable ya que pueden ser análisis de software, contenidos teóricos o guías de procesos que reúnen teoría y tutoriales.  

## Índice de cápsulas    

<ul class="pages">
  {% for page in site.pages %}
  {% if page.categoria == "capsula" %}

      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><a href="{{ page.url }}">{{ page.title }}</a></li>
   {% endif %}
      {% endfor %}
</ul>