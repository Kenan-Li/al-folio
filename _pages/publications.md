---
layout: page
permalink: /publications/
title: Publications
description: My publications in reversed chronological order.
years: [2010, 2015, 2016, 2018, 2019, 2020, 2021, 2022, 2023]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
