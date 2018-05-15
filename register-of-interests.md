---
layout: page
title: Register of Interests
heading: Register of Interests
permalink: /register-of-interests/
---

<table id="minutes-table">
  <tr>
    <th>Declared</th>
    <th>Officer</th>
    <th>Matter</th>
  </tr>
  {% for interest in site.register-of-interests %}
    <tr>
      <td>{{ interest.declared | date: "%-d %B %Y"}}</td>
      <td>{{ interest.officer }}</td>
      <td>{{ interest.matter }}</td>
    </tr>
    <tr>
      <td colspan="3">{{ interest.content }}</td>
    </tr>
  {% endfor %}
</table>
