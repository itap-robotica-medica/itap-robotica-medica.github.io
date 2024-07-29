---
title: "ITAP Medical Robotics - Projects"
layout: gridlay
excerpt: "ITAP Medical Robotics -- Projects"
sitemap: false
permalink: /projects/
---


# Projects

<div class="container mt-4">
    <div class="accordion" id="projectsAccordion">

        <!-- Category 1 -->
        <div class="card">
            <div class="card-header" id="headingOne">
                <h2 class="mb-0">
                    <button class="btn btn-link btn-block text-left" type="button" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                        Category 1
                    </button>
                </h2>
            </div>
            <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#projectsAccordion">
                <div class="card-body">
                    {% assign number_printed = 0 %}
                    {% for proj in site.data.projectlist %}
                        {% if proj.category == "Category 1" %}
                            <div style="padding-left:15px;padding-right:15px;">
                                <div class="well" style="overflow: hidden;">
                                    <img src="{{ site.url }}{{ site.baseurl }}/images/projpic/{{ proj.image }}" class="img-responsive" width="33%" style="float: left" />
                                    <pubtit><a href="{{ site.url }}{{ site.baseurl }}/projects/{{ proj.url }}">{{ proj.title }}</a></pubtit>
                                    <p>{{ proj.description }}</p>
                                </div>
                            </div>
                            {% assign number_printed = number_printed | plus: 1 %}
                        {% endif %}
                    {% endfor %}
                </div>
            </div>
        </div>

        <!-- Category 2 -->
        <div class="card">
            <div class="card-header" id="headingTwo">
                <h2 class="mb-0">
                    <button class="btn btn-link btn-block text-left collapsed" type="button" data-toggle="collapse" data-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                        Category 2
                    </button>
                </h2>
            </div>
            <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo" data-parent="#projectsAccordion">
                <div class="card-body">
                    {% assign number_printed = 0 %}
                    {% for proj in site.data.projectlist %}
                        {% if proj.category == "Category 2" %}
                            <div style="padding-left:15px;padding-right:15px;">
                                <div class="well" style="overflow: hidden;">
                                    <img src="{{ site.url }}{{ site.baseurl }}/images/projpic/{{ proj.image }}" class="img-responsive" width="33%" style="float: left" />
                                    <pubtit><a href="{{ site.url }}{{ site.baseurl }}/projects/{{ proj.url }}">{{ proj.title }}</a></pubtit>
                                    <p>{{ proj.description }}</p>
                                </div>
                            </div>
                            {% assign number_printed = number_printed | plus: 1 %}
                        {% endif %}
                    {% endfor %}
                </div>
            </div>
        </div>

        <!-- Category 3 -->
        <div class="card">
            <div class="card-header" id="headingThree">
                <h2 class="mb-0">
                    <button class="btn btn-link btn-block text-left collapsed" type="button" data-toggle="collapse" data-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                        Category 3
                    </button>
                </h2>
            </div>
            <div id="collapseThree" class="collapse" aria-labelledby="headingThree" data-parent="#projectsAccordion">
                <div class="card-body">
                    {% assign number_printed = 0 %}
                    {% for proj in site.data.projectlist %}
                        {% if proj.category == "Category 3" %}
                            <div style="padding-left:15px;padding-right:15px;">
                                <div class="well" style="overflow: hidden;">
                                    <img src="{{ site.url }}{{ site.baseurl }}/images/projpic/{{ proj.image }}" class="img-responsive" width="33%" style="float: left" />
                                    <pubtit><a href="{{ site.url }}{{ site.baseurl }}/projects/{{ proj.url }}">{{ proj.title }}</a></pubtit>
                                    <p>{{ proj.description }}</p>
                                </div>
                            </div>
                            {% assign number_printed = number_printed | plus: 1 %}
                        {% endif %}
                    {% endfor %}
                </div>
            </div>
        </div>

    </div>
</div>

{% assign number_printed = 0 %}
{% for proj in site.data.projectlist %}

<div style="padding-left:15px;padding-right:15px;">
<div class="well" style="overflow: hidden;">
<img src="{{ site.url }}{{ site.baseurl }}/images/projpic/{{ proj.image }}" class="img-responsive" width="33%" style="float: left" />
<pubtit><a href="{{ site.url }}{{ site.baseurl }}/projects/{{ proj.url }}">{{ proj.title }}</a></pubtit>
<p>{{ proj.description }}</p>
</div>
</div>


{% endfor %}

<p> &nbsp; </p>
