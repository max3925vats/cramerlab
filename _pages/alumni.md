---
title: "Cramer Lab - Alumni"
layout: textlay
excerpt: "Cramer Lab: Alumni"
sitemap: false
permalink: /alumni.html
---

### Alumni
---
{% for alumni in site.data.alumni %}

<b>{{alumni.name}}</b>: "{{alumni.thesis}}", degree conferred in {{alumni.date}}. {{alumni.info}}.

{% endfor %}
