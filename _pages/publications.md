---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2013, 2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, 1999, 1998, 1997, 1996, 1995, 1993, 1992]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year" style="color:#6A6B6B;">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
