---
layout: default
title: "note"
permalink: /note/
---

# Kategori Note

<ul>
  {% for post in site.posts %}
    {% if post.categories contains 'note' %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>

