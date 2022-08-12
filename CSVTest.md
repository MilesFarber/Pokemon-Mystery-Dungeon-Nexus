---
title: Table test
---

{% assign row = site.data.profiles[0] %}
{{ row | inspect }}

{% assign row = site.data.profiles[0] %}
{% for pair in row %}
  {{ pair | inspect }}
{% endfor %}

<table>
  {% for row in site.data.profiles %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>

<table>
    <thead>
        <tr>
            <th colspan="2">The table header</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>The table body</td>
            <td>with two columns</td>
        </tr>
    </tbody>
</table>
