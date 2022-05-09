---
layout: page
permalink: /publications/
title: Publications
description: A list of published work, as well as papers under review or in preparation.
years: [2022,2021,2020,2017]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
