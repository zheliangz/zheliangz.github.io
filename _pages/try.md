---
layout: page
title: try
permalink: /try/
description: A growing collection of your cool projects.
nav: false
nav_order:
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="publications">
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {% endfor %}
