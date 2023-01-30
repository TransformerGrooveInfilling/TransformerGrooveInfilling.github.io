---
layout: page
title: Random Low
description: InfillingRL
importance: 1
category: InfillingRL
---

Below are the examples for the InfillingRandomLow model

More examples can be found `https://anonusergit.github.io/assets/wav/`


    ---
    GT: Ground Truth (Complete Version from which small percentage of events are removed)
    IRL: Generated events
    IRL (Mix): Generated events mixed with input
    ---


`NOTE` that the generated events are quieter than the ground truth. No adjustment was made for creating the mixed versions to demonstrate the performance of the model in replicating velocities. 


<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  border: 1px solid black;
  padding: 4px;
  text-align: center;
  width: 10%;
}

th {
  background-color: lightgray;
}
</style>

<table>
  <thead>
    <tr>
      <th>INDEX</th>
      <th>GT</th>
      <th>IRL</th>
      <th>IRL (Mix)</th>
    </tr>
  </thead>
  <tbody>
    {% for x in (0..60) %}
      {% if forloop.index0 % 5 == 0 %}
    <tr>
      <td>{{ x }}</td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomLow/{{ x }}_A_target.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomLow/{{ x }}_B_irl_prd.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomLow/{{ x }}_C_irl_mix.wav"></audio></td>
    </tr>
      {% endif %}
    {% endfor %}
  </tbody>
</table>




