---
layout: page
permalink: /publications/
title: publications
description: <h6>Please see <b><a href='https://scholar.google.ca/citations?user=NDGuxa8AAAAJ&hl=en&oi=ao'>Google Scholar Profile</a></b> for an up-to-date list.</h6>
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 1999]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
