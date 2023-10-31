---
layout: page
permalink: /publications/
title: Publications
description: '*'Corresponding author  '†'Advisor as the first author
years: [2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
  <h2>Preprints</h2>
  {% bibliography -f preprint %}
</div>
