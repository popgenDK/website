---
title: "EPIC seminar series"
layout: gridlay
excerpt: "..."
sitemap: false
permalink: /EPIC_seminar/
---

## Next up

{% assign number_printed = 0 %}
{% for talk in site.data.EPIC_seminar %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if talk.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <meta charset="utf-8"> 
  <pubtit>{{ talk.title }}</pubtit>
  <a href="{{ talk.link.url }}" target="blank" >
     <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ talk.image }}"  title="{{ talk.abstract }}" class="img-responsive" width="33%" style="float: left" />
   </a>
  <p>{{ talk.description }}</p>
  <p><em>{{ talk.authors }}</em></p>
  <p><strong><a href="{{ talk.link.url }}">{{ talk.link.display }}</a></strong></p>
  {% if talk.github %}
  <p><strong><a href="{{ talk.github }}">Code used in paper</a></strong></p>
  {% endif %}
  <p class="text-danger"><strong> {{ talk.news1 }}</strong></p>
  <p> {{ talk.news2 }}</p>
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

{% for talk in site.data.EPIC_seminar %}
  
  {{pub_number_printed}} <b>{{ talk.title }} </b> <br />
  <em>{{ talk.author }} </em><br /><a href="{{ talk.link.url }}">{{ talk.link.display }}</a>

{% assign pub_number_printed = pub_number_printed | plus: 1 %}

{% endfor %}
