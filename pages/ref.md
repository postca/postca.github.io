---
layout: default
title: "note"
permalink: /note/
---

# Kategori Note

{% if paginator %}
    <div class="blog-posts hfeed index-post-wrap" id="post-list">
        {% for post in paginator.posts %}
            {% include post_list_item.html %}
        {% endfor %}
    </div>

    <div class="blog-pager" id="blog-pager">
        {% if paginator.next_page %}
            <a class="blog-pager-older-link" href="{{ paginator.next_page_path | relative_url }}">
                Load More
            </a>
        {% else %}
            <span class="no-more">That is All</span>
        {% endif %}
    </div>
{% endif %}

