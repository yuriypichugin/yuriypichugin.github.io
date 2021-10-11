---
layout: page
permalink: /publications/
order: 3
title: publications and preprints
description: "* denotes shared first co-authorship. # denotes corresponding authorship."
years: [2021, 2020, 2019, 2017, 2015, 2012]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
