---
layout: page
title: Structural documents
heading: Structural documents
permalink: /structural-documents/
---

<table id="minutes-table">
  {% for document in site.structural-documents %}
    <tr>
      <td><a href="{{ document.url }}">{{ document.title }}</a></td>
    </tr>
  {% endfor %}
</table>
