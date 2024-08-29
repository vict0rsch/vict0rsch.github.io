---
layout: page
permalink: /publications/
title: Publications
description: "Publications by categories in reversed chronological order. See <a href='https://scholar.google.com/citations?user=mKLme1kAAAAJ&hl=fr' rel='noreferrer noopener' target='_blank'>Google Scholar</a>."
years: [2024, 2023, 2022, 2021, 2020, 2019]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
