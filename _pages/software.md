---
title: "Albrechtsen Lab - Software"
layout: gridlay
excerpt: "Albrechtsen Lab -- Software."
sitemap: false
permalink: /software/
---
# Software


{% assign number_printed = 0 %}
{% for software in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if software.website %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ software.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ software.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ software.description }}</p>
  <p><em>{{ software.authors }}</em></p>
  <p><strong><a href="{{ software.link.url }}">{{ software.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ software.news1 }}</strong></p>
  <p> {{ software.news2 }}</p>
 </div>
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

<p> &nbsp; </p>
