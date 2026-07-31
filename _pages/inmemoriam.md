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

<div class="row hidden-xs">

{% if even_odd == 0 %}
<div class="col-sm-10">
  <div class="row">
    <div class="col-sm-3">
      <p><img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="85%" style="float: left; margin-bottom: 20px" /></p> 
    </div>
    <div class="col-sm-9">
      <h4>{{ member.name }}</h4>
      <p><i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> --></i></p> 
      <p><i>{{ member.datebirth }} - {{ member.datepassing }}</i></p> 
      <div>{{ member.paragraph }}</div> 
    </div>
  </div>
</div>
<div class="col-sm-2">
</div>
{% endif %}

{% if even_odd == 1 %}
<div class="col-sm-2">
</div>
<div class="col-sm-10">
  <div class="row">
    <div class="col-sm-9">
      <h4 class="text-right">{{ member.name }}</h4>
      <p class="text-right"><i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> --></i></p>
      <p class="text-right"><i>{{ member.datebirth }} - {{ member.datepassing }}</i></p> 
      <div class="text-right">{{ member.paragraph }}</div> 
    </div> 
    <div class="col-sm-3">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="85%" style="float: right; margin:16px 6px 22px 20px; box-shadow: -2px 2px 5px #888" />
    </div>
  </div>
</div>
{% endif %}

{% assign number_printed = number_printed | plus: 1 %}

</div>

{% endfor %}

{% assign number_printed = 0 %}
{% for member in site.data.in_memoriam %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row visible-xs-block">

{% if even_odd == 0 %}
<div class="col-sm-10">
  <div class="row">
    <div class="col-sm-3">
      <p><img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="85%" style="float: left; margin-bottom: 20px" /></p> 
    </div>
    <div class="col-sm-9">
      <h4>{{ member.name }}</h4>
      <p><i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> --></i></p> 
      <p><i>{{ member.datebirth }} - {{ member.datepassing }}</i></p> 
      <div>{{ member.paragraph }}</div> 
    </div>
  </div>
</div>
<div class="col-sm-2">
</div>
{% endif %}

{% if even_odd == 1 %}
<div class="col-sm-2">
</div>
<div class="col-sm-10">
  <div class="row">
    <div class="col-sm-3">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="85%" style="float: right; margin:16px 6px 22px 20px; box-shadow: -2px 2px 5px #888" />
    </div>
    <div class="col-sm-9">
      <h4 class="text-right">{{ member.name }}</h4>
      <p class="text-right"><i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> --></i></p>
      <p class="text-right"><i>{{ member.datebirth }} - {{ member.datepassing }}</i></p> 
      <div class="text-right">{{ member.paragraph }}</div> 
    </div> 
  </div>
</div>
{% endif %}



{% assign number_printed = number_printed | plus: 1 %}

</div>

{% endfor %}

<center>
  <a href="/team">
  <div>

  ←        Current members

  </div></a>
</center>

<br>
