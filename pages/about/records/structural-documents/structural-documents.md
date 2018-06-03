---
layout: page
title: Structural documents
permalink: /structural-documents/
parent: "Records"
---

## Articles of Association

<table class="documents-table">
  <tr class="document-entry">
    <td><a href="{{ site.baseurl }}/articles-of-association/">Articles of Association</a></td>
  </tr>
</table>

## Committee terms of reference

<table class="documents-table">
  {% for tor in site.terms-of-reference %}
    <tr class="document-entry">
      <td><a href="{{ tor.url }}">{{ tor.title }}</a></td>
    </tr>
  {% endfor %}
</table>
