---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order. "*" Indicates equal contributions.
conference_years: [2021, 2020]
workshop_years: [2020, 2019]
nav: true
---

<h1>Conference Papers</h1>

<div class="publications">

{% for y in page.conference_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


<h1>Workshop Papers</h1>

<div class="publications">

{% for y in page.workshop_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshop_papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
