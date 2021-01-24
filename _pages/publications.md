---
layout: page
permalink: /publications/
title: publications
description: Publications in reverse chronological order starting with pre-prints.
years: [2020, 2019, 2017]
order: 7
---

<h3 class="year">Preprints</h3>
{% bibliography -f preprints %}

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h3 class="year">Scopus papers, proceedings, posters and others</h3>

