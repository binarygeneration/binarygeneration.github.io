---
layout: contact
title: "Team"
subtitle: "(Humans of the project)"
permalink: /contacts/
feature-img: "assets/img/pexels/travel.jpeg"
tags: [Contacts]
---

Here are the wonderful people working on this project.


Jump to [Faculty](#faulty), [Researchers](#Researchers).

## Researchers
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-8 clearfix">
  <!--<img src="{{ site.url }}{{ site.baseurl }}/assets/img/memberpics/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />-->
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>Email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

{% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

{% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

{% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

{% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Faculty
{% assign number_printed = 0 %}
{% for member in site.data.faculty %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-8 clearfix">
  <!--<img src="{{ site.url }}{{ site.baseurl }}/assets/img/memberpics/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />-->
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>Email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

{% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

{% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

{% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

{% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

{% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
 
