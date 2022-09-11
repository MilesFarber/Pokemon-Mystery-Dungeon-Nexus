---
layout: default
title: LearnDex
permalink: LearnDex
---
{% assign row = site.data.learnsets[0] %}
{% for row in site.data.learnsets %}{% if forloop.first %}{% for pair in row %}|{{ pair[0] }}{% endfor %}{% endif %}|
{% for pair in row %}|{{ pair[1] }}{% endfor %}{% endfor %}|
