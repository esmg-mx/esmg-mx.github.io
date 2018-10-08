---
title: "ESMG-MX: News"
layout: textlay
excerpt: "The Earth-Science Modeling Group."
published: true
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p><b>{{ article.date }}</b> <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
