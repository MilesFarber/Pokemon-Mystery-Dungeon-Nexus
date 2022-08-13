# Characters

{% assign row = site.data.profiles[0] %}
{% for row in site.data.profiles %}{% if forloop.first %}{% for pair in row %}|{{ pair[0] }}{% endfor %}{% endif %}|
{% for pair in row %}|{{ pair[1] }}{% endfor %}{% endfor %}|
