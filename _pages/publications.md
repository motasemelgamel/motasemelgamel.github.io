---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2024, 2023]
nav: True
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<!-- <h3>Submitted</h3>
<h2 class="year">{{y}}</h2>
  <br>
  {% bibliography -f papers_submitted %}

<br> -->

<!-- <h3>Published</h3> -->
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>