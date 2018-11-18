---
layout: page
title: Blog
permalink: /blog/
parent: "Our work"
order: 4
---

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      {% for category in post.categories %}
        <span class="post-category">{{ category | upcase }}</span>
      {% endfor %}
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      {% if post.author %}
        <p class="post-meta">{{ post.author }} | {{ post.date | date: "%-d %B %Y"}}</p>
      {% endif %}
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
