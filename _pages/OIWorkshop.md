---
title: "Open Institute Workshop"
layout: gridlay
excerpt: "Open Institute Workshop"
sitemap: false
permalink: /workshop/
---


# Workshop: Introduction to population genomics in wildlife conservation
<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="4000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
        <li data-target="#carousel" data-slide-to="4"></li>
        <li data-target="#carousel" data-slide-to="5"></li>
        <li data-target="#carousel" data-slide-to="6"></li>
    </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/caucasian.phased.haplonet.merged.anno.png" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/finstructure.gif" alt="Slide 2" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/check.anno.png" alt="Slide 3" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/tp.png" alt="Slide 4" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/sikoraPlot.jpeg" alt="Slide 5" />
        </div>       
         <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/plaque.png" alt="Slide 6" />
        </div>
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>


## General info

**Date:** August 7-9, 2024 <br/>
**Place:** ... Kilifi, Kenya  <br/>
**Organized by:** The Department of Biology, University of Copenhagen <br/>
**Price:** ... <br/>
**Includes:** Two meals per day, breakfast and lunch <br/>
**Sign up:** ...  <br/>
**Contact:** For questions write to ...  <br/>

# Content
...
Each session (morning and afternoon) contains a lecture (about 45 minutes) and one or two practicals (45 or 2x45 minutes each). Every afternoon after the session there will be a research talk with focus on the topics of the day. 

## Intended Learning Outcome
- Understand what NGS short-read data looks like when it comes from the sequencer, and have an overview of what needs to be done to it before population genetic analyses can be done. 
- Understand how to estimate genome-wide heterozygosity, and what to use it for in conservation biology. 
- Be able to estimate ROHs and inbreeding coefficients, and understand the potential negative consequences of autozygosity.
- Understand the concept of population structure and be able to use PCA, admixture analyses and Fst to quantify and interpret it.
- Understand how population structure analyses can be used to define conservation units and inform translocation schemes.

## Instructors

{% assign number_printed = 0 %}
{% for yml in site.data.workshop %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if yml.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <h2>{{ yml.name }}</h2>
  <pubtit>{{ yml.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ yml.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ yml.description }} <strong><a href="{{ yml.website }}">website</a></strong></p>  
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



## Time and place

...
You should bring a laptop to the course. We will log into a remote server from the laptop so any laptop will do regardless of operating system.


# Program

### Wednesday
    - Morning session: Introduction to NGS data, SNP calling and genotype calling  -  Anders
    - Afternoon session: Genetic diversity, heterozygosity  -  Rasmus

### Thursday
    - Morning session: ROHs, inbreeding  -  Anubhab
    - Afternoon session: annotation and genetic load, synonymous/nonsynonymous mutations  -  Anubhab
    
### Friday
    - Morning session: Population structure, gene flow and admixture.  -  Rasmus
    - Afternoon session: PCA, Fst  -  Anders
    
