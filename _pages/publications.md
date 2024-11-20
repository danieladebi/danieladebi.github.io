---
layout: page
permalink: /publications/
title: Publications
description: \* denotes equal contribution
years: [2024] #[1967, 1956, 1950, 1935, 1905] put years in order that you want displayed
nav: true
nav_order: 2 
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
