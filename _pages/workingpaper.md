---

layout: page
permalink: /workingpapers/
title: Working Papers
description: Working papers in various topics.
years: [2022]
nav: false
nav_order: 1
display_categories: [Monetary, Environment]

---
<!-- _pages/workingpaper.md -->
<div class="workingpapers">
<!-- Display categorized projects -->
{%- if site.enable_project_categories and page.display_categories %}
{%- for category in page.display_categories %}
<h2 class="category">{{ category }}</h2>
{%- assign categorized_wp = site.projects | where: "category", category -%}
{%- assign sorted_wp = categorized_wp | sort: "importance" %}

{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
