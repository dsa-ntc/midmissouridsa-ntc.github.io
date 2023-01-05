---
layout: page
title: "Our Work"
permalink: /our-work/
---

<div>
    {% for item in site.data.nav.our-work %}
        <h3>{{ item.title }}</h3>
        {% for entry in item.pages %}
            <a href="{{ entry.url }}">
                <h4>{{ entry.title }}</h4>
            </a>
        {% endfor %}
    {% endfor %}
</div>
