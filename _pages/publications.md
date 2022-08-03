---
layout: page
permalink: /publications/
title: RESEARCH
description: 
years: [1967, 1956, 1950, 1935, 1905]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h1>Publications</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1>Working Papers</h1>

{% bibliography -f papers %}
  
</div>
