---
layout: page
permalink: /publications/
title: Publications
description:
years: [2022, 2023, 2012, 1935, 1905]
nav: false
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers_alt -q @*[year={{y}}]* %}
{% endfor %}

</div>