---
layout: default
title: Characters
permalink: Characters
---

# Comparisons

{% assign row = site.data.comparisons[0] %}
{% for row in site.data.comparisons %}{% for pair in row %}{% if forloop.first %}### {{ pair[0] }} {% endif %} {{ pair[1] }} {% endfor %}{% endfor %}

# Character sheets

{% assign row = site.data.characters[0] %}
{% for row in site.data.characters %}{% if forloop.first %}{% for pair in row %}|{{ pair[0] }}{% endfor %}{% endif %}|
{% for pair in row %}|{{ pair[1] }}{% endfor %}{% endfor %}|
