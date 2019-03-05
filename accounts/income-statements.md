---
layout: accounts
title: Income Statements
---

<ul>
  <li><a href="{{ site.url }}/accounts/summary-of-accounts.html">Lifetime statement</a></li>
  {% for statement in site.income-statements %}
    <li><a href="{{ statement.url }}">{{ statement.from | date: "%-d %B %Y" }} to {{ statement.to | date: "%-d %B %Y" }}</a></li>
  {% endfor %}
</ul>
