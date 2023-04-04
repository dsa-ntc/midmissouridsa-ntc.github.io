---
layout: page
title: Working Groups
permalink: /working-groups/
---

<div>
  {% for entry in site.data.nav.working-groups.pages %}
  <a href="{{ entry.url }}">
    <h4>{{ entry.title }}</h4>
  </a>
  {% endfor %}
</div>
