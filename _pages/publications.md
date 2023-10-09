---
layout: page
permalink: /publications/
title: publications
description: <p>Please refer to my  <a href="https://scholar.google.ca/citations?user=NDGuxa8AAAAJ&hl=en">Google Scholar Profile</a> for a complete list. </p>
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
