---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2025, 2024, 2023]
nav: True
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h6>* Equal contribution</h6>
<br>

<h2 class="section">Submitted</h2>
{% bibliography -f papers_submitted %}

<br>
<h2 class="section">Published</h2>
{%- for y in page.years %}
  <h2 class="year{% if forloop.first %} first-year{% endif %}">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
