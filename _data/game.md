---
title: "Game Review / Game Design"
layout: archive
permalink: /game/
author_profile: true
---

{% assign game_posts = site.posts | where_exp: "item", "item.categories contains 'game'" %}
{% if game_posts.size > 0 %}
{% for post in game_posts %}
- **[{{ post.title }}]({{ post.url | relative_url }})** — *{{ post.date | date: "%Y-%m-%d" }}*
{% endfor %}
{% else %}
*Chưa có bài viết nào trong mục này.*
{% endif %}
