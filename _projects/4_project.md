---
layout: page
title: Random High
description: InfillingRandomHigh
importance: 1
category: Validation Set Examples
---

Below are the examples for the InfillingRandomHigh model

More examples can be found at [https://github.com/AnonUserGit/AnonUserGit.github.io/tree/master/assets/wav](https://github.com/AnonUserGit/AnonUserGit.github.io/tree/master/assets/wav)

    ---
    GT: Ground Truth (Complete Version from which large percentage of events are removed)
    IRH: Generated events
    IRH (Mix): Generated events mixed with input
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
      <th>IRH</th>
      <th>IRH (Mix)</th>
    </tr>
  </thead>
  <tbody>
    {% for x in (0..60) %}
      {% if forloop.index0 % 5 == 0 %}
    <tr>
      <td>{{ x }}</td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomHigh/{{ x }}_A_target.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomHigh/{{ x }}_B_ir_prd.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingRandomHigh/{{ x }}_C_mix.wav"></audio></td>
    </tr>
      {% endif %}
    {% endfor %}
  </tbody>
</table>


