---
layout: accounts
title: Profit & loss statements
---

<ul>
  <li><a href="{{ site.url }}/accounts/summary-of-accounts.html">Lifetime statement</a></li>
  {% for statement in site.profit-and-loss-statements %}
    <li><a href="{{ statement.url }}">{{ statement.from | date: "%-d %B %Y" }} to {{ statement.to | date: "%-d %B %Y" }}</a></li>
  {% endfor %}
</ul>
