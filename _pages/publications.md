---
# Disclaimer: This page was written and revised with assistance from
# OpenAI Codex (GPT-6). The author remains responsible for verifying all results.
layout: page
permalink: /publications/
title: Publications
description: 
nav: True
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h6><sup>*</sup>Equal contribution</h6>
<br>

<h2 class="section">Submitted</h2>
{% bibliography -f papers_submitted %}

<br>
<h2 class="section">Published</h2>
<!-- Derive year headings from published entries, with the newest year first. -->
{% bibliography -f papers --group_by year --group_order descending %}

</div>
