---
layout: page
title: Minutes
heading: Minutes
permalink: /minutes/
---

<table id="minutes-table">
  <tr>
    <th nowrap="nowrap">Date</th>
    <th>Description</th>
  </tr>
  {% for minute in site.minutes %}
    <tr>
      <td nowrap="nowrap">{{ minute.date | date: "%-d %B %Y"}}</td>
      <td><a href="{{ minute.url }}">{{ minute.title }}</a></td>
    </tr>
  {% endfor %}
</table>
