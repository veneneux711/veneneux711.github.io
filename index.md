---
layout: default
---

# Welcome to _veneneux's corner

---

## Gunpla
{% assign gunpla_posts = site.posts | where_exp: "item", "item.categories contains 'gunpla'" %}
{% if gunpla_posts.size > 0 %}
  {% for post in gunpla_posts %}
    - **[{{ post.title }}]({{ post.url | relative_url }})** — *{{ post.date | date: "%Y-%m-%d" }}*
  {% endfor %}
{% else %}
  *Chưa có bài viết nào trong mục này.*
{% endif %}

---

## Game Review & Game Design
{% assign game_posts = site.posts | where_exp: "item", "item.categories contains 'game'" %}
{% if game_posts.size > 0 %}
  {% for post in game_posts %}
    - **[{{ post.title }}]({{ post.url | relative_url }})** — *{{ post.date | date: "%Y-%m-%d" }}*
  {% endfor %}
{% else %}
  *Chưa có bài viết nào trong mục này.*
{% endif %}

---

## Random Rants
{% assign rant_posts = site.posts | where_exp: "item", "item.categories contains 'rant'" %}
{% if rant_posts.size > 0 %}
  {% for post in rant_posts %}
    - **[{{ post.title }}]({{ post.url | relative_url }})** — *{{ post.date | date: "%Y-%m-%d" }}*
  {% endfor %}
{% else %}
  *Chưa có bài viết nào trong mục này.*
{% endif %}

---

### 📝 Tất cả bài viết
{% for post in site.posts %}
  - **[{{ post.title }}]({{ post.url | relative_url }})** <small>({{ post.categories | join: ", " }})</small> — *{{ post.date | date: "%Y-%m-%d" }}*
{% endfor %}
