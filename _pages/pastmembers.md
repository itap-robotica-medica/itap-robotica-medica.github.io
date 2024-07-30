---
title: "ITAP Medical Robotics - Past members"
layout: gridlay
excerpt: "ITAP Medical Robotics - Past members"
sitemap: false
permalink: /team/past/
---

# Past members

{% assign number_printed = 0 %}
{% for member in site.data.past_members %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="40%" style="float: left" />
  <h4>{{ member.name }}</h4>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd != 0 %}
</div>
{% endif %}
