---
layout: page
title: Minutes
permalink: /minutes/
parent: "Records"
---

<table class="documents-table">
  {% for minute in site.minutes reversed %}
    <tr class="document-entry">
      <td nowrap="nowrap">{{ minute.date | date: "%-d %B %Y"}}</td>
      <td><a href="{{ minute.url }}">{{ minute.title }}</a>
      {% if minute.layout == "meeting" %}
        | <span class="toggle-agenda">show agenda</span>
        <ul class="minutes-table-agenda">
          {% for item in minute.agenda %}
            <li>{{ item }}</li>
          {% endfor %}
        </ul>
      {% endif %}
      </td>
    </tr>
  {% endfor %}
</table>

<script src="{{ site.url }}/assets/jquery-3.3.1.min.js"></script>

<script>
  $(".toggle-agenda").click(function() {
    if ($(this).html() == "show agenda") {
      $(this).html("hide agenda");
      $(this).next(".minutes-table-agenda").show();
    } else {
      $(this).html("show agenda");
      $(this).next(".minutes-table-agenda").hide();
    };
  });
</script>
