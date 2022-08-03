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

<h1>Job Market Paper</h1>
## Job Market Paper
  
{% bibliography -f jobmarketpaper %}

<h1>workingpapers</h1>

{% bibliography -f workingpapers %}
  
 
<h1>workinprogress</h1>

{% bibliography -f workinprogress %}
  
<h1>publishedpapers</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f publishedpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>
