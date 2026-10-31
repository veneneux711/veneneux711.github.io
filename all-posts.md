---
title: "Tất cả bài viết"
layout: archive
permalink: /all-posts/
author_profile: true
---

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url | relative_url }})** — *{{ post.date | date: "%Y-%m-%d" }}*
{% endfor %}
