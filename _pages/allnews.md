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
<img src="{{ site.url }}{{ site.baseurl }}/images/newspic/{{ proj.image }}" class="img-responsive" width="33%" style="float: left" />
<p>{{ proj.date }}</p> 
<p><em>{{ proj.headline }}</em></p>
<p>{{ proj.link }}</p>
</div>
</div>


{% endfor %}

<p> &nbsp; </p>
