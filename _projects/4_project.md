---
layout: page
title: InfillingRandomHigh
description: InfillingRH
importance: 1
category: InfillingRH
---

Below are the examples for the InfillingRandomHigh model

More examples can be found [here](https://anonusergit.github.io/assets/wav/)


    ---
    GT: Ground Truth (Complete Version from which large percentage of events are removed)
    IRH: Generated events
    IRH (Mix): Generated events mixed with input
    ---

`NOTE` that the generated events are quieter than the ground truth. No adjustment was made for creating the mixed versions to demonstrate the `poor performance` of the model in replicating velocities. 


<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  border: 1px solid black;
  padding: 8px;
  text-align: center;
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
      <th>IKS</th>
      <th>IKS (Mix)</th>
    </tr>
  </thead>
  <tbody>
    {% for x in (0..115) %}
    <tr>
      <td>{{ x }}</td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomHigh/{{ x }}_A_target.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomHigh/{{ x }}_B_ks_prd.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomHigh/{{ x }}_C_ks_mix.wav"></audio></td>
    </tr>
    {% endfor %}
  </tbody>
</table>







