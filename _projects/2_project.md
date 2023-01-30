---
layout: page
title: InfillingKicksAndSnares
description: InfillingKS
importance: 1
category: InfillingKS
---

Below are the examples for the InfillingKicksAndSnares model

More examples can be found https://anonusergit.github.io/assets/wav/


    ---
    GT: Ground Truth (Complete Version from which Kicks and Snares were removed during training)
    IKS: Generated Kicks and Snares (Audio Input)
    IKS (Mix): Generated Kicks and Snares Mixed with Inputs (Audio Input)
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
	{% if forloop.index0 % 5 == 0 %}
    <tr>
      <td>{{ x }}</td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingKicksAndSnares/{{ x }}_A_target.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingKicksAndSnares/{{ x }}_B_ks_prd.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingKicksAndSnares/{{ x }}_C_ks_mix.wav"></audio></td>
    </tr>
    {% endfor %}
  </tbody>
</table>







