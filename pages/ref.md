---
layout: default
title: "ref"
permalink: /ref/
---

# Kategori Android

{% for post in site.categories.ref %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}
