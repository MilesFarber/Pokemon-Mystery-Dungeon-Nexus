# PMDItems

{% assign row = site.data.pmditems[0] %}
{% for row in site.data.pmditems %}{% if forloop.first %}{% for pair in row %}|{{ pair[0] }}{% endfor %}{% endif %}|
{% for pair in row %}|{{ pair[1] }}{% endfor %}{% endfor %}|
