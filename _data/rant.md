---
title: "Random Rants"
layout: archive
permalink: /rant/
author_profile: true
---

{% assign rant_posts = site.posts | where_exp: "item", "item.categories contains 'rant'" %}
{% if rant_posts.size > 0 %}
{% for post in rant_posts %}
- **[{{ post.title }}]({{ post.url | relative_url }})** — *{{ post.date | date: "%Y-%m-%d" }}*
{% endfor %}
{% else %}
*Chưa có bài viết nào trong mục này.*
{% endif %}
