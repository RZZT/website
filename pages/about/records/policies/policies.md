---
layout: page
title: Policies
permalink: /policies/
parent: "Records"
---

<table class="documents-table">
  {% for policy in site.policies %}
    <tr class="document-entry">
      <td><a href="{{ policy.url }}">{{ policy.title }}</a></td>
    </tr>
  {% endfor %}
</table>
