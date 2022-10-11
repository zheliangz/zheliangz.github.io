---
layout: page
permalink: /publications/
title: Publications
description: Publications in various topics.
nav: false
years:[2022]
nav_order:
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
