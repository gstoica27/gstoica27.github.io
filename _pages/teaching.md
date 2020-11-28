---
layout: page
permalink: /teaching/
title: teaching
description: Courses I have assisted teaching.
years: [2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f teaching -q @*[year={{y}}]* %}
{% endfor %}

</div>
