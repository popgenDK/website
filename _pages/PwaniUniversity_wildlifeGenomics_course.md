---
title: "Wildlife Genomics Course"
layout: gridlay
excerpt: "Wildlife Genomics Course"
sitemap: false
permalink: /wildlife_genomics_course/
---


# Course: Introduction to wildlife genomics
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

**Date:** August 12-23, 2024 <br/>
**Place:** Pwani University, Kilifi, Kenya  <br/>
**Organized by:** Pwani University, University of Copenhagen, the African BioGenome Project. <br/>
**Price:** Free <br/>
**Includes:** All teaching, breakfast and lunch on course days. Accommodation is NOT included. <br/>
**Sign up:** Via African BioGenome Project (AfricaBP) Open Institute East and Central African Regional Workshop 2024 ([link]( https://docs.google.com/forms/d/e/1FAIpQLSfzZxCkLfyPRSr7qBZbCAbW80VApLepzkD_9JZijcHUlTJ9fg/viewform))  <br/>
**Contact:** For questions write to sammywambua@gmail.com anubhabkhan@gmail.com <br/>

# Content
The course is a comprehensive introduction to population genetics and the use of genomics tools especially in the context of wildlife research and conservation. All sessions will have hands-on data analysis.
Topics: fundamental population genetics, Next-generation sequencing, genomic data analysis, application of genomics to wildlife census, trafficking and population management

## Intended Learning Outcome
- Importance of population genetics and genomics in wildlife conservation and management
- Understand what NGS short-read data looks like when it comes from the sequencer, and have an overview of what needs to be done to it before population genetic analyses can be done. 
- Understand various measures of genetic diversity, inbreeding, population structure, relatedness
- Estimate demographic history and its consequnces for population survival or extinction
- Application of genomics in wildlife management
- Metagenomes and their analysis

## Instructors

{% assign number_printed = 0 %}
{% for yml in site.data.course %}

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
    
