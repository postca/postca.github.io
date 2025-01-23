---
layout: default
title: "note"
permalink: /note/
---

# Kategori Note

{% if paginator %}
    <div class="blog-posts hfeed index-post-wrap" id="post-list">
        {% for post in site.posts %}
    {% if post.categories contains 'note' %}
            {% include post_list_item.html %}
         {% endif %}
  {% endfor %}
    </div>

{% if paginator %}
<div class='blog-pager' id='blog-pager'>
  {% if paginator.next_page %}
    <a class='blog-pager-older-link btn load-more' href='{{ paginator.next_page_path | relative_url }}' id='supermag-pro-load-more-link'>
      Load More
    </a>
    <span class='loading'><div class='loader'></div></span>
    <span class='no-more btn load-more' style='display:none;'>That is All</span>
  {% else %}
    <span class='no-more btn load-more show'>That is All</span>
  {% endif %}
</div>
{% endif %}
