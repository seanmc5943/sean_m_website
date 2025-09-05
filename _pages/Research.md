---
layout: page
permalink: /research/
title: Research
description: 
years: [2026, 2025, 2024, 2023]
nav: true
nav_order: 2
---
<!-- _pages/Research.md -->

## Working Papers

<div class="publications">
{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

