---
title: "News"
layout: textlay
excerpt: "Cramer Lab at RPI."
sitemap: false
permalink: /news.html
---

### News
---

{% for article in site.data.news %}
{% if forloop.index == 21 %}
​    {% break %}
  {% endif %}
<p style="text-align:justify;">{{ article.date }} - <em>{{ article.headline }}</em></p>
{% endfor %}
