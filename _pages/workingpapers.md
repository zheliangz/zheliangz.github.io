---
layout: page
title: Working Papers
permalink: /workingpapers/
description: Working papers in various topics.
nav: false
display: [Monetary Economics, Environmental Economics]
horizontal: false
---



<!-- _pages/workingpapers.md -->
<div class="publications">


{%- for y in page.display%}
<h2 class="topic">{{ y }}</h2>

{% bibliography -f papers -q @*[topic={{y}}]* %}

{% endfor %}


</div>
