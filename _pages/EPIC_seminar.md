---
title: "EPIC seminar series"
layout: gridlay
excerpt: "..."
sitemap: false
permalink: /EPIC_seminar/
---

## Next up

{% assign number_printed = 0 %}
{% for date in site.data.EPIC_seminar %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if date.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <meta charset="utf-8"> 
  <pubtit>{{ date.title }}</pubtit>
  <a href="{{ date.link.url }}" target="blank" >
     <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ date.image }}"  title="{{ date.description }}" class="img-responsive" width="33%" style="float: left" />
   </a>
  <p>{{ date.description }}</p>
  <p><em>{{ date.speaker1 }}</em></p>
  <p><em>{{ date.speaker2 }}</em></p>
  <p><strong><a href="{{ date.link.url }}">{{ date.link.display }}</a></strong></p>
  {% if date.github %}
  <p><strong><a href="{{ date.github }}">Code used in paper</a></strong></p>
  {% endif %}
  <p class="text-danger"><strong> {{ date.news1 }}</strong></p>
  <p> {{ date.news2 }}</p>
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


# Full List of talks


{% assign pub_number_printed = 1 %}

{% for date in site.data.EPIC_seminar %}
  
  {{pub_number_printed}} <b>{{ date.title1 }} </b> <br />
  <em>{{ date.speaker1 }} </em><br /><a href="{{ date.link.url }}">{{ date.link.display }}</a>
  {{pub_number_printed}} <b>{{ date.title2 }} </b> <br />
  <em>{{ date.speaker2 }} </em><br /><a href="{{ date.link.url }}">{{ date.link.display }}</a>

{% assign pub_number_printed = pub_number_printed | plus: 1 %}

{% endfor %}
