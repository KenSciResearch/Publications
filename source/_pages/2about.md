---
layout: distill
title: other
permalink: /other

profile:
  align: right
  image: 

news: false  # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---



<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f kensci -q @*[year={{y}}]* %}
{% endfor %}

</div>
