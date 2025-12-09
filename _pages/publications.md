---
layout: page
permalink: /publications/
title: PUBLICATIONS
description: Peer reviewed publications by categories in reversed chronological order.
years: [2025, 2023, 2022, 2019, 2018]
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
