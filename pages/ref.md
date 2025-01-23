---
layout: default
title: "note"
permalink: /note/
---

# Kategori Note


    <div class="blog-posts hfeed index-post-wrap" id="post-list">
        {% for post in site.posts %}
    {% if post.categories contains 'note' %}
            {% include post_list_item.html %}
         {% endif %}
  {% endfor %}
    </div>
