---
layout: page
permalink: /publications/
title: publications
description: 
years: [2024,2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
You can see the most updated version in [Google Scholar](https://scholar.google.com/citations?user=9LtfMfMAAAAJ&hl=en)
<div class="publications">

Note: * denotes equal contribution.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
