---
title: "ITAP Medical Robotics - Team"
layout: gridlay
excerpt: "ITAP Medical Robotics - Team"
sitemap: false
permalink: /team/in-memoriam/
---



# In Memoriam

{% assign number_printed = 0 %}
{% for member in site.data.in_memoriam %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

{% if even_odd == 0 %}
<div class="col-sm-8">
  <p><img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="50%" style="float: left" /></p> 
  <h4>{{ member.name }}</h4>
  <p><i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> --></i></p> 
</div>
{% endif %}

{% if even_odd == 1 %}
<div class="col-sm-4">
</div>
<div class="col-sm-8">
  <div class="w-50 pull-left">
  <h4>{{ member.name }}</h4>
  <p><i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> --></i></p>
  </div> 
  <div class="w-50 pull-right">
  <p> <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="50%" style="float: right" /></p> 
  </div>
</div>
{% endif %}



{% assign number_printed = number_printed | plus: 1 %}

</div>

{% endfor %}

<center>
  <a href="/team">
  <div>

  Current members        →

  </div></a>
</center>

<br>
