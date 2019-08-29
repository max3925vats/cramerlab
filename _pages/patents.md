---
title: "Cramer Lab - Patents"
layout: textlay
excerpt: "Patents"
sitemap: false
permalink: /patents.html
---

### Patents
---

{% for patent in site.data.patents %}

<a href="{{ patent.link }}">US Patent # {{patent.number}}</a> "{{ patent.title }}", {{ patent.authors }}, ({{ patent.year }})

{% endfor %}
