---
layout: page
title: 文章归档
permalink: /archive
---

## 所有文章

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%Y年%m月%d日" }}</span>
      {{ post.title }}
    </li>
  {% endfor %}
</ul>

<style>
.post-list {
  list-style: none;
  padding-left: 0;
}
.post-list li {
  margin-bottom: 15px;
  border-bottom: 1px solid #eee;
  padding-bottom: 10px;
}
.post-date {
  display: inline-block;
  width: 120px;
  color: #666;
}
</style>
