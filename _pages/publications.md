---
layout: page
permalink: /publications/
title: publications
description: Publications by categories in chronological order. # generated by jekyll-scholar.
years: [2022, 2018, 2017, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006, 2005, 2004] # 2021, 2020, 2019, 2016,  2003
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
