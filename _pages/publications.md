---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
years: [2024, 2022, 2021]
---

<!-- _pages/publications.md -->
<div class="publications">

{% bibliography %}

{%- for y in page.years %}
  <h2 class="year" style="color: blue">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
