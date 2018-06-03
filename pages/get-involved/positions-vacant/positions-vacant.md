---
layout: page
title: Positions vacant
permalink: /positions-vacant/
parent: "Get involved"
order: 5
---

{% if site.data.positions-vacant.length < 1 %}
  There are currently no positions vacant.
{% else %}
  {% for position in site.data.positions-vacant %}
  <p>{{ position.advertised | date: "%A %-d %B %Y"}}</p>
  <p><strong>{{ position.position }} | {{ position.salary }}</strong></p>
  <p>{{ position.description }}</p>
  <p><strong>Apply to:</strong> <a href="mailto:{{ position.contact }}">{{ position.contact }}</a></p>
  {% if forloop.last %}
  {% else %}
<hr/>
  {% endif %}
{% endfor %}
{% endif %}
