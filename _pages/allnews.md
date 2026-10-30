---
title: "News"
layout: textlay
sitemap: true
permalink: /allnews.html
---

## News

{% for article in site.data.news %}
<div style="text-align:justify"><strong>{{ article.date }}</strong> <br> {{ article.headline | markdownify | remove: '<p>' | remove: '</p>' }}</div>
<br>
{% endfor %}
