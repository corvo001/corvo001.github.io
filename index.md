---
layout: home
author_profile: true
title: "Soy Daniel Cuervo"
excerpt: "Integración de software y ciencia. De la idea al prototipo funcional."
header:
  overlay_color: "#000"
  overlay_filter: "0.25"
---

<h2>Recent Posts</h2>
{% assign posts_home = site.posts | where: "show_on_home", true %}
{% for post in posts_home %}
  <article>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
  </article>
{% endfor %}