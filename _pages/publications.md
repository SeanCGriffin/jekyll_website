---
layout: page
permalink: /publications/
title: publications
description: A subset of my "first-author" refereed publications and conference proceedings. 
years: [2017, 2015]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>