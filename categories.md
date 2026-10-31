---
title: "Bài viết theo Danh mục"
layout: archive
permalink: /categories/
author_profile: true
---

<h2 id="gunpla">🤖 Gunpla</h2>
{% assign gunpla_posts = site.posts | where_exp: "item", "item.categories contains 'gunpla'" %}
{% if gunpla_posts.size > 0 %}
  {% for post in gunpla_posts %}
    <article class="archive__item">
      <h3 class="archive__item-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <p class="page__meta"><i class="far fa-clock" aria-hidden="true"></i> {{ post.date | date: "%Y-%m-%d" }}</p>
    </article>
  {% endfor %}
{% else %}
  <p><em>Chưa có bài viết nào trong mục này.</em></p>
{% endif %}

<hr>

<h2 id="game">🎮 Game Review / Game Design</h2>
{% assign game_posts = site.posts | where_exp: "item", "item.categories contains 'game'" %}
{% if game_posts.size > 0 %}
  {% for post in game_posts %}
    <article class="archive__item">
      <h3 class="archive__item-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <p class="page__meta"><i class="far fa-clock" aria-hidden="true"></i> {{ post.date | date: "%Y-%m-%d" }}</p>
    </article>
  {% endfor %}
{% else %}
  <p><em>Chưa có bài viết nào trong mục này.</em></p>
{% endif %}

<hr>

<h2 id="rant">💬 Random Rants</h2>
{% assign rant_posts = site.posts | where_exp: "item", "item.categories contains 'rant'" %}
{% if rant_posts.size > 0 %}
  {% for post in rant_posts %}
    <article class="archive__item">
      <h3 class="archive__item-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <p class="page__meta"><i class="far fa-clock" aria-hidden="true"></i> {{ post.date | date: "%Y-%m-%d" }}</p>
    </article>
  {% endfor %}
{% else %}
  <p><em>Chưa có bài viết nào trong mục này.</em></p>
{% endif %}
