---
layout: page
title: Working Papers
permalink: /workingpapers/
description: Working papers in various topics.
nav: false
nav_order:
display_1: [Monetary Policy]
display_2: [Environmental Economics]
years_1: [2022, 1950]
horizontal: false
---

<!-- pages/try.md -->


<div class="publications">


{%- for category in page.display_1%}
<h2 class="category">{{ category }}</h2>
{%- for y in page.years_1 %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
{% endfor %}


{%- for category in page.display_2%}
 <h2 class="category">{{ category }}</h2>

{% endfor %}

</div>
