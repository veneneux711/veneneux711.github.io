---
title: "Gunpla"
layout: archive
permalink: /gunpla/
author_profile: true
---

{% assign gunpla_posts = site.posts | where_exp: "item", "item.categories contains 'gunpla'" %}
{% if gunpla_posts.size > 0 %}
{% for post in gunpla_posts %}
- **[{{ post.title }}]({{ post.url | relative_url }})** — *{{ post.date | date: "%Y-%m-%d" }}*
{% endfor %}
{% else %}
*Chưa có bài viết nào trong mục này.*
{% endif %}
