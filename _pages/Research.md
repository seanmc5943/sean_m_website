---
layout: page
permalink: /research/
title: Research
description: 
years: [2024, 2023]
nav: true
nav_order: 2
---
<!-- _pages/Research.md -->

## Working Papers

<div class="publications">
{% bibliography -f papers -q @*[year={{y}}]* %}
{%- for y in page.years %}
  <h2 class="year"></h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

