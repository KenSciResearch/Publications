---
layout: about
title: about
permalink: /
description: List of KenSci Publications

profile:

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page

years: [2021, 2020, 2019, 2018, 2017, 2016, 2014, 2013]
---


<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f kensci -q @*[year={{y}}]* %}
{% endfor %}

</div>