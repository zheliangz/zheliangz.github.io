---
layout: page
title: Working Papers
permalink: /workingpapers/
description: Working papers in various topics.
nav: false
#nav_order:
display: [Monetary Economics, Environmental Economics]
horizontal: false
---

<!-- pages/try.md -->


<div class="publications">


{%- for y in page.display%}
<h2 class="topic">{{ y }}</h2>

{% bibliography -f papers -q @*[topic={{y}}]* %}

{% endfor %}




</div>
