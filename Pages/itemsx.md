---
layout: default
title: ItemDex (Special)
permalink: ItemDex(Special)
---
{% assign row = site.data.itemsx[0] %}
{% for row in site.data.itemsx %}{% if forloop.first %}{% for pair in row %}|{{ pair[0] }}{% endfor %}{% endif %}|
{% for pair in row %}|{{ pair[1] }}{% endfor %}{% endfor %}|
