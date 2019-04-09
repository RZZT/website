---
layout: page
title: Officers
permalink: /officers/
parent: "About"
order: 6
---

RZZT is governed by up to three Directors. The Directors make decisions affecting all aspects of the Company. Most of the routine day-to-day administrative tasks are carried out by the Company Secretary, who is appointed by the Directors.

{% assign grouped_officers = site.data.officers | group_by: "role" %}
{% for group in grouped_officers %}
  {% assign officers = group.items | sort: "surname" %}
  {% for officer in officers %}
<div class="officer-profile">
  <div>
    <strong>{{ officer.forename }} {{ officer.surname }}</strong><br>
    <em>{{ officer.role }}</em><br>
    {{ officer.bio }}<br>
  </div>
</div>
  {% endfor %}
{% endfor %}
