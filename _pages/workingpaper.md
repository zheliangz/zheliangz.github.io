---

layout: page
permalink: /workingpapers/
title: Working Papers
description: Working papers by categories in reversed chronological order.
years: [2022]
nav: false
nav_order: 1

---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
