---
layout: page
permalink: /publications/
title: Publications
description: "* indicates equal contribution."
years: [2025]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

Please see <a href="https://scholar.google.com/citations?user=Ed7h-uMAAAAJ"> Google Scholar</a> for a complete and up-to-date list of publications.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
