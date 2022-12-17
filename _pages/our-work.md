---
layout: page
title: "Our Work"
permalink: /our-work/
---

<div>
    {% for item in site.data.nav.our-work %}
        <h2>{{ item.title }}</h2>
        {% for entry in item.pages %}
            <a href="{{ entry.url }}">
                <h3>{{ entry.title }}</h3>
            </a>
        {% endfor %}
    {% endfor %}
</div>
