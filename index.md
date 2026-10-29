---
layout: default
---

# Welcome to _veneneux's corner

Góc nhỏ chia sẻ về Gunpla/Model Kits, tư duy Game Design và những dòng suy nghĩ ngẫu hứng.

---

## Gunpla
<ul>
  {% for post in site.posts %}
    {% if post.categories contains 'gunpla' %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%Y-%m-%d" }}</small>
      </li>
    {% endif %}
  {% endfor %}
</ul>

---

## Game/Game Design
<ul>
  {% for post in site.posts %}
    {% if post.categories contains 'game' %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%Y-%m-%d" }}</small>
      </li>
    {% endif %}
  {% endfor %}
</ul>

---

## Random Rants
<ul>
  {% for post in site.posts %}
    {% if post.categories contains 'rant' %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%Y-%m-%d" }}</small>
      </li>
    {% endif %}
  {% endfor %}
</ul>

---

### Tất cả bài viết
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
</ul>
