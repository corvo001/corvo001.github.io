---
layout: home
author_profile: true
title: "Soy Daniel Cuervo"
excerpt: "Integración de software y ciencia. De la idea al prototipo funcional."
header:
  overlay_color: "#000"
  overlay_filter: "0.25"
  overlay_image: /assets/images/header.png   # tu banner
---

{% assign featured_post = site.posts | where: "title", "Presentación del Portafolio de Cuervo" | first %}
{% if featured_post %}
  {% include archive-single.html post=featured_post %}
{% endif %}