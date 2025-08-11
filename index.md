---
layout: single
author_profile: true
title: ""
pagination: false
---

## Posts

{%- comment -%}
Primero intentamos por slug fijo (recomendado).
Si no lo encuentra, hacemos fallback por título.
{%- endcomment -%}
{% assign featured_post = site.posts | where: "slug", "presentacion-del-portafolio-de-cuervo" | first %}
{% if featured_post %}
  {% include archive-single.html post=featured_post type="list" %}
{% else %}
  {% assign featured_post = site.posts | where: "title", "Presentación del Portafolio de Cuervo" | first %}
  {% if featured_post %}
    {% include archive-single.html post=featured_post type="list" %}
  {% else %}
    <p>No se encontró el post de presentación.</p>
  {% endif %}
{% endif %}
