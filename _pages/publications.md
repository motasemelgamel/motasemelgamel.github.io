---
layout: page
permalink: /publications/
title: Publications
description:
years: []
nav: True
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h3>Submitted</h3>
  {% bibliography -f papers_submitted %}

<h3>Published</h3>
  {% bibliography -f papers %}

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

