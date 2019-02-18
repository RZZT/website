---
layout: page
title: Media
permalink: /media/
parent: "About"
order: 0
---

<ul class="post-list">
  {% for post in site.categories["media"] %}
    <li>
      {% for category in post.categories %}
        <span class="post-category">{{ category | upcase }}</span>
      {% endfor %}
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="post-meta">
        {% if post.author %}
          {{ post.author }} |
        {% endif %}
        {{ post.date | date: "%-d %B %Y"}}
      </p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
