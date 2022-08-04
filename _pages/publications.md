---
layout: page
permalink: /publications/
title: RESEARCH
description: 
years: [2022, 2023, 2024]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
  
<h1>Job Market Paper</h1>

{% bibliography -f papers -q @*[progress=jobmarketpaper]* %} 

<h1>Working Papers</h1>

{% bibliography -f papers -q @*[progress=workingpaper]* %}
  
<h1>Select Work in Progress</h1>

{% bibliography -f papers -q @*[progress=workinprogress]* %}
  
<h1>Publications</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[progress=published && year={{y}}]* %}
{% endfor %}


  
</div>
