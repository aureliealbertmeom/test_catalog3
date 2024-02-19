---
layout: default
---

# MEOM catalog

This is where you can find all the informations about the available datasets extracted from simulations performed by MEOM

<table>
  {% for e in site.data.datasets %}
      {% if forloop.first == true %}
      <tr>
      {% for item in e %}
          <th>{{item[0]}}</th>
      {% endfor %}
      </tr>
      {% endif %}
      <tr>
      {% for item in e %}
          <td>{{item[1]}}</td>
      {% endfor %}
      </tr>
  {% endfor %}
</table>
