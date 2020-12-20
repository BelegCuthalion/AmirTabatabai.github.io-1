---
layout: page
permalink: /publications/
title: Publications
description: publications by categories in reversed chronological order.
years: [1935, 2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
