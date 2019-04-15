---
layout: page
title: Officers
permalink: /officers/
parent: "About"
order: 6
---

RZZT is governed by a Board of Directors who oversee the general operation of the Company. They appoint a Managing Director to conduct the day-to-day management of the Company, and a Company Secretary to perform routine administrative tasks.

{% for officer in officers %}
  <div class="officer-profile">
    <div>
      <strong>{{ officer.forename }} {{ officer.surname }}</strong><br>
      <em>{{ officer.role }}</em><br>
      {{ officer.bio }}<br>
    </div>
  </div>
{% endfor %}
