---
layout: default
title: "note"
permalink: /note/
---

# Kategori Android

{% for post in site.categories.note %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}
