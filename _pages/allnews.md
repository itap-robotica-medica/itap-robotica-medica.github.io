---
title: "News"
layout: gridlay
excerpt: "ITAP Medical Robotics -- News"
sitemap: false
permalink: /allnews.html
---

# News
<!--
{% for article in site.data.news %}
<p>{{ article.date }}
<br>
<em>{{ article.headline }}</em>
<br>
{{ article.link }} </p>
{% endfor %}

# Projects

{% assign number_printed = 0 %} -->

{% for proj in site.data.news %}

  <div style="padding-left:15px;padding-right:15px;">
  <div class="well" style="overflow: hidden;">
    
  {% if proj.image != NULL %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/newspic/{{ proj.image }}" class="img-responsive" width="50%" style="float: left" />
  {% endif %}
  
  <p>{{ proj.date }}</p> 
  
  <p><em>{{ proj.headline }}</em></p>

  {% if proj.spotify != NULL %}
  <div>{{ proj.spotify }}<\div>
  {% endif %}
  
  {% if proj.link != NULL %}
  <p>{{ proj.link }}</p>

  {% if proj.link1 != NULL %}
  <p>{{ proj.link1 }}</p>
  {% if proj.link2 != NULL %}
  <p>{{ proj.link2 }}</p>
  {% if proj.link3 != NULL %}
  <p>{{ proj.link3 }}</p>
  {% if proj.link4 != NULL %}
  <p>{{ proj.link4 }}</p>
  {% endif %}
  {% endif %}
  {% endif %}
  {% endif %}

  </div>
  </div>

{% endfor %}

<p> &nbsp; </p>
