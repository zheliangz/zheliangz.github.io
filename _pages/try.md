---
layout: page
title: try
permalink: /try/
description: A growing collection of your cool projects.
nav: false
nav_order:
display_1: [work]
display_2: [fun]
years: [2022]
horizontal: false
---

<!-- pages/try.md -->


<div class="publications">


{%- for category in page.display_1%}
<h2 class="category">{{ category }}</h2>
{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

{% endfor %}

{%- for category in page.display_2%}
 <h2 class="category">{{ category }}</h2>

{% endfor %}
