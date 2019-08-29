---
title: "Cramer Lab - Gallery"
layout: gallery
excerpt: "Cramer Lab - Gallery"
sitemap: false
permalink: /gallery
---

<h3 class="page-description text-center">The Cramer Lab Gallery</h3>
<div class="tz-gallery">
<div class="row">
{% for pic in site.data.gallery %}

<div class="col-sm-3">
<div class="thumbnail">
<a class="lightbox" href="{{site.url}}{{site.baseurl}}/assets/images/Gallery/{{pic.photo}}"><img src="{{site.url}}{{site.baseurl}}/assets/images/Gallery/{{pic.photo}}" alt="{{pic.title}}"></a>
<div class="caption">
<h3>{{pic.caption}}</h3>
<p>{{pic.info}}</p>
</div>
</div>
</div>

{% endfor %}

</div>
</div>
