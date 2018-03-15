---
layout: page
title: Policies
heading: Policies
permalink: /policies/
---

<table id="minutes-table">
  {% for document in site.policies %}
    <tr>
      <td><a href="{{ document.url }}">{{ document.title }}</a></td>
    </tr>
  {% endfor %}
</table>
