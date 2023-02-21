---
layout: page
permalink: /publications/
title: selected publications | <a href='https://ui.adsabs.harvard.edu/public-libraries/DCWz-kzgTj2eow6FLxBXSw'>ADS</a>
years:
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

