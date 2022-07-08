---
layout: page
title: try
permalink: /try/
description: A growing collection of your cool projects.
nav: false
nav_order:
display_categories: [work, fun]
years: [2022]
horizontal: false
---

<!-- pages/try.md -->
<h2 class="category">{{ work }}</h2>

<div class="publications">
{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>


<h2 class="category">{{ fun }}</h2>

<div class="publications">
{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
