---
layout: page
permalink: /talks/
title: talks
description: 
years: [2025, 2024, 2022, 2021]
nav: true
---

<div class="talks">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>