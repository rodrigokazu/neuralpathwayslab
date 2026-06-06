---
title: "News"
layout: textlay
sitemap: true
permalink: /allnews.html
---

## News

{% for article in site.data.news %}
<p style="text-align:justify"><strong>{{ article.date }}</strong> <br> {{ article.headline | markdownify}}</p>
<br>
{% endfor %}
