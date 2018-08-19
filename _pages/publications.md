---
layout: page
permalink: /publications/
title: publications
description: My published research from undergrad and beyond
years: [2017, 2014]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
