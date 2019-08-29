---
title: "Cramer Lab - Publications"
layout: gridlay
excerpt: "Cramer Lab -- Publications."
sitemap: false
permalink: /publications.html
---

### Publications
---
#### Highlights

(For a full list go to [Google Scholar](https://scholar.google.com/citations?user=x1aWa9sAAAAJ&hl=en&oi=ao))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">

  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/pubpic/{{ publi.image }}" class="img-responsive" width="20%" style="float: left" />
  <pubtit>{{ publi.title }}</pubtit>

  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

---
### Latest...
<br />

{% assign counter = 0 %}

{% for publi in site.data.publist %}

{{ publi.title }}. <br />
  <em>{{ publi.authors }} </em><br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}, ({{ publi.year }})</a>

{% assign counter = counter | plus: 1 %}
{% if counter == 10 %}
{% break %}
{% endif %}
{% endfor %}

---
<p> More on  [Google Scholar](https://scholar.google.com/citations?user=x1aWa9sAAAAJ&hl=en&oi=ao).</p>
