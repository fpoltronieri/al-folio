---
layout: page
permalink: /publications/
title: Publications
description: List of pubblications.
years: [2023,2022, 2021, 2020, 2019, 2018]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

RoamML MILCOM paper [Download]({{ site.url }}/assets/pdf/roamml_milcom_paper.pdf).

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
