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
    </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/wildebeest_admix.png" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/wildebeest_het.png" alt="Slide 2" />
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
**Place:** Pwani University, Kilifi, Kenya  <br/>
**Organized by:** Pwani University, University of Copenhagen, the African BioGenome Project. <br/>
**Price:** Free <br/>
**Includes:** All teaching, breakfast and lunch on workshop days. Accommodation is NOT included. <br/>
**Sign up:** Via African BioGenome Project (AfricaBP) Open Institute East and Central African Regional Workshop 2024 ([link]( https://docs.google.com/forms/d/e/1FAIpQLSfzZxCkLfyPRSr7qBZbCAbW80VApLepzkD_9JZijcHUlTJ9fg/viewform)  <br/>
**Contact:** For questions write to ...  <br/>

# Content
The course is a comprehensive introduction to a number of topics and common research tools used in population genetic analyses of next-generation sequencing (NGS) data with a focus on applying them in conservation. Topics include: genetic data overview, estimating genetic diversity, inbreeding and population structure. There will be an emphasis on how to apply these concepts and analyses in wildlife conservation. We will introduce the theoretical concepts, but the main focus is practical use of the methods. Lectures will be combined with hands-on computer exercises and research talks providing examples of case studies. 

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

The workshop is part of the ABP Open Institute East and Central African Regional Workshop 2024. It will take place from Wednesday August 7th to Friday August 9th 2024 at Pwani University, Kilifi, Kenya [add full address]. All lectures and computer exercises will take place in room xxx. This includes research talks. 
You are required to bring a laptop to the course. We will log into a remote server from the laptop, so any laptop will do regardless of operating system. 



# Program (preliminary)

### Wednesday
    - Morning session: Introduction to NGS data, SNP calling and genotype calling  -  Anders
    - Afternoon session: Genetic diversity, heterozygosity  -  Rasmus

### Thursday
    - Morning session: ROHs, inbreeding  -  Anubhab
    - Afternoon session: annotation and genetic load, synonymous/nonsynonymous mutations  -  Anubhab
    
### Friday
    - Morning session: Population structure, gene flow and admixture.  -  Rasmus
    - Afternoon session: PCA, Fst  -  Anders
    
