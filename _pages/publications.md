---
layout: page
permalink: /publications/
title: publications
description:
years: [2026, 2025, 2024, 2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h2>Articles</h2>
{%- for y in page.years %}
  {% bibliography -f papers -q @article[year={{ y }}] %}
{%- endfor %}

<h2>Proceedings</h2>
{%- for y in page.years %}
  {% bibliography -f papers -q @inproceedings[year={{ y }}] %}
{%- endfor %}

</div>