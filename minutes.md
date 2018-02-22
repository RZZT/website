---
layout: page
title: Minutes
heading: Minutes
permalink: /minutes/
---

<table id="minutes-table">
  <tr>
    <th>Date</th>
    <th>Description</th>
  </tr>
  {% for minute in site.minutes %}
    <tr>
      <td>{{ minute.date | date: "%-d %B %Y"}}</td>
      <td><a href="{{ minute.url }}">{{ minute.title }}</a></td>
    </tr>
  {% endfor %}
</table>
