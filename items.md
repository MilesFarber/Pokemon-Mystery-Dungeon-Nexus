---
layout: default
title: ItemDex
permalink: ItemDex
---
{% assign row = site.data.items[0] %}
{% for row in site.data.items %}{% if forloop.first %}{% for pair in row %}|{{ pair[0] }}{% endfor %}{% endif %}|
{% for pair in row %}|{{ pair[1] }}{% endfor %}{% endfor %}|
