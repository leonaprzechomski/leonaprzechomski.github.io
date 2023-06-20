---
layout: page
permalink: /publications/
title: publications
description: Here you will soon see publications.
years: [2023]
nav: true
nav_order: 1
---

Will this change show up and if yes, why?

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
