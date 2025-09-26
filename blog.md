---
layout: default
title: Blog
---

# 글 목록

<ul>
  {% for post in site.posts %}
    <li>
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <span>{{ post.date | date: "%Y년 %m월 %d일" }}</span>
    </li>
  {% endfor %}
</ul>
