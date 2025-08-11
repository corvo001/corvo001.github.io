---
layout: single
author_profile: true
title: ""
pagination: false
---

## Posts

{%- comment -%} 1) Buscar por categoría 'Presentación' (con y sin tilde) {%- endcomment -%}
{% assign featured_post = site.posts | where_exp: "p", "p.categories contains 'Presentación'" | first %}
{% if featured_post == nil %}
  {% assign featured_post = site.posts | where_exp: "p", "p.categories contains 'Presentacion'" | first %}
{% endif %}

{%- comment -%} 2) Fallback por slug fijo {%- endcomment -%}
{% if featured_post == nil %}
  {% assign featured_post = site.posts | where: "slug", "presentacion-del-portafolio-de-cuervo" | first %}
{% endif %}

{%- comment -%} 3) Fallback por título exacto {%- endcomment -%}
{% if featured_post == nil %}
  {% assign featured_post = site.posts | where: "title", "Presentación del Portafolio de Cuervo" | first %}
{% endif %}

{% if featured_post %}
  {% include archive-single.html post=featured_post type="list" %}
{% else %}
  <p>No se encontró el post de presentación.</p>
{% endif %}
