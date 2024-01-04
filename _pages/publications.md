---
layout: page
permalink: /publications/
title: Publications
description:
years: [2023,2022, 2021, 2020, 2019,2018,2017,2016]
nav: true
nav_order: 2
---
**Full List** on <a href='https://scholar.google.com/citations?user=_OH8SF0AAAAJ&hl=en'>Google Scholar</a>


<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
