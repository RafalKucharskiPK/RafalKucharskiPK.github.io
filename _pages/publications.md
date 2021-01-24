---
layout: page
permalink: /publications/
title: publications
description: Journal publications (IF only) in reverse chronological order starting with pre-prints.
years: [2020, 2019, 2017]
order: 7
---

Selected IF papers and pre-prints (submitted) only, for full list pleasee see my scholar.

<h3 class="year">Preprints</h3>
{% bibliography -f preprints %}

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}



