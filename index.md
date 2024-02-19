---
layout: default
---

# MEOM catalog

This is where you can find all the informations about the available datasets extracted from simulations performed by MEOM

<table>
      <tr>
          <th> Name of dataset</th>
          <th> Configuration</th>
          <th> Simulation</th>
          <th> Region</th>
          <th> Period</th>
          <th> Frequency</th>
          <th> Variables</th>
          <th> Size</th>
          <th> Opendap link</th>
          <th> Cal path</th>
          <th> GRICAD path</th>
          <th> Adastra path</th>
      </tr>  
  {% for e in site.data.datasets %}
      <tr>
          <th>{{ e.title}</th>
          <th>{{ e.config}</th>
          <th>{{ e.simu}</th>
          <th>{{ e.region}</th>
          <th>{{ e.period}</th>
          <th>{{ e.freq}</th>
          <th>{{ e.vars}</th>
          <th>{{ e.size}</th>
          <th>{{ e.opendap}</th>
          <th>{{ e.cal1}</th>
          <th>{{ e.gricad}</th>
          <th>{{ e.adastra}</th>
      </tr>
  {% endfor %}
</table>
