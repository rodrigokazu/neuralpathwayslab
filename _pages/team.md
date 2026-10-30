---
title: "Neural Pathways Lab - Team"
layout: gridlay
sitemap: true
permalink: /team/
---

<style>
.np-initials {
  float: left;
  width: 25%;
  aspect-ratio: 1 / 1;
  margin-right: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #e8eef5;
  color: #337ab7;
  font-weight: 600;
  font-size: 26px;
  letter-spacing: 1px;
}
</style>

<div style="margin-top: 45px;">

### Team

</div>

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix" style="text-align: justify;"> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left">
  <h4>{{ member.name }}</h4>
  {% if member.scholar %}<a href="{{ member.scholar }}" target="_blank"><i class="fa fa-graduation-cap" style="font-size:13px; color:black"></i></a>{% endif %}
  <a href="mailto:{{ member.email }}"><i class="fa fa-envelope" style="font-size:13px; color:black"></i></a>
  
  <i>{{ member.info }}<br></i>

  {% if member.number_educ == 1 %}
  <p> {{ member.education1 }} </p>
  {% endif %}

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


### Key collaborators

{% assign number_printed = 0 %}
{% for member in site.data.key_collaborators %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix" style="text-align:justify;">
  {% if member.photo %}<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />{% else %}<span class="np-initials">{{ member.initials }}</span>{% endif %}
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}{% if member.email %}
  <br>email: {{ member.email }}{% endif %}</i>

  {% if member.number_educ == 1 %}
  <p> {{ member.education1 }} </p>
  {% endif %}

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

### Collaborators

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix" style="text-align:justify;">
  {% if member.photo %}<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />{% else %}<span class="np-initials">{{ member.initials }}</span>{% endif %}
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}{% if member.email %}
  <br>email: {{ member.email }}{% endif %}</i>

  {% if member.number_educ == 1 %}
  <p> {{ member.education1 }} </p>
  {% endif %}

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

{% if site.data.former_collaborators.size > 0 %}
### Former Collaborators

{% assign number_printed = 0 %}
{% for member in site.data.former_collaborators %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix" style="text-align:justify;">
  {% if member.photo %}<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />{% else %}<span class="np-initials">{{ member.initials }}</span>{% endif %}
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}{% if member.email %}
  <br>email: {{ member.email }}{% endif %}</i>

  {% if member.number_educ == 1 %}
  <p> {{ member.education1 }} </p>
  {% endif %}

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
{% endif %}
