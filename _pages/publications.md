---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2020, 2018, 2017]
nav: true

---

#### Preprints

<div class="publications">

{% for y in page.years %}
  {% bibliography -f preprint -q @*[year={{y}}]* %}
{% endfor %}

</div>


#### Journal Papers

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journalpubs -q @*[year={{y}}]* %}
{% endfor %}

</div>

#### Conference Papers

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f confpubs -q @*[year={{y}}]* %}
{% endfor %}

</div>


