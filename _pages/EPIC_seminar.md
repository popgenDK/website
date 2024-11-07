---
title: "EPIC seminar series"
layout: gridlay
excerpt: "..."
sitemap: false
permalink: /EPIC_seminar/
---

# Next up

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
  <p><em><b>{{ date.day }}</b></em></p>
  <p><em><b>{{ date.title1 }}</b></em></p>
  <p><em>{{ date.speaker1 }}</em></p>
  <p><em><b>{{ date.title2 }}</b></em></p>
  <p><em>{{ date.speaker2 }}</em></p>
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

{% for date in site.data.EPIC_seminar %}

  <b>{{ date.day }} </b> <br />
  <b>{{ date.title1 }} </b> <br />
  <em>{{ date.speaker1 }} </em> <br />
  <b>{{ date.title2 }} </b> <br />
  <em>{{ date.speaker2 }} </em><br />
  
{% endfor %}
