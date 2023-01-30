---
layout: page
title: InfillingClosedHH
description: InfillingClosedHH (Symbolic Vs Audio Versions)
importance: 1
category: InfillingClosedHH
---

Below Are the examples for the Infilling HiHats Models comparing the symbolic model (IHS) vs the audio one (IH). 


More examples can be found https://anonusergit.github.io/assets/wav/




    ---
    GT: Ground Truth (Complete Version from which HiHats were removed during training)
    IH: Generated Hihats (Audio Input)
    IHS: Generated Hihats (Symbolic Input)
    IH (Mix): Generated HiHats Mixed with Inputs (Audio Input)
    IHS: Generated HiHats Mixed with Inputs (Symbolic Input)
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
      <th>IH</th>
      <th>IHS</th>
      <th>IH (Mix)</th>
      <th>IHS (Mix)</th>
    </tr>
  </thead>
  <tbody>
    {% for x in (0..115) %}
      {% if forloop.index0 %% 5 == 0 %}
    <tr>
      <td>{{ x }}</td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingClosedHH/{{ x }}_A_target.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingClosedHH/{{ x }}_B_ih_prd.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingClosedHH/{{ x }}_B_ihs_prd.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingClosedHH/{{ x }}_C_ih_mix.wav"></audio></td>
      <td><audio controls><source src="{{ site.baseurl }}/assets/wav/InfillingClosedHH/{{ x }}_C_ihs_mix.wav"></audio></td>
    </tr>
      {% endif %}
    {% endfor %}
  </tbody>
</table>








