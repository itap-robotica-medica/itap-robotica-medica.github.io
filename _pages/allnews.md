---
title: "News"
layout: textlay
excerpt: "ITAP Medical Robotics -- News"
sitemap: false
permalink: /allnews.html
---

# News

<style>
    .news-container {
        display: flex;
        flex-wrap: wrap;
    }

    .news-item {
        flex: 0 0 20%; /* Adjust the percentage to control column width */
        padding: 10px;
        box-sizing: border-box;
    }

    .news-image {
        max-width: 100%;
        height: auto;
    }
</style>

<div class="news-container">
    {% for article in site.data.news %}
    <div class="news-item">
        <img class="news-image" src="image_url_here" alt="a">
    </div>
    <div class="news-item">
        <p>{{ article.date }}<br>
        <em>{{ article.headline }}</em><br>
        {{ article.link }}</p>
    </div>
    {% endfor %}
</div>

{% for article in site.data.news %}
<p>{{ article.date }}
<br>
<em>{{ article.headline }}</em>
<br>
{{ article.link }} </p>
{% endfor %}
