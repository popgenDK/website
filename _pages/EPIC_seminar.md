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
  <pubtit>{{ date }}</pubtit>
  <p><em>{{ date.speaker1 }}</em></p>
  <p><em>{{ date.title1 }}</em></p>
  <p><em>{{ date.speaker2 }}</em></p>
  <p><em>{{ date.title2 }}</em></p>
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
