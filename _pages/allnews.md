---
title: "News"
layout: textlay
excerpt: "Albrechtsen Lab."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br> {{ article.headline | markdownify}}</p>
{% endfor %}

<a class="twitter-timeline" href="https://twitter.com/PopGenDK?ref_src=twsrc%5Etfw">Tweets by PopGenDK</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> 


Twitter feed placeholder:



<section id="main-description">
  <div class="container">
    <div class="row">
      <div class="col-md-8">
        ...
      </div>
      <div class="col-md-4">
        <div>
          <a class="twitter-timeline" href="https://twitter.com/CodeForBuffalo?ref_src=twsrc%5Etfw">Tweets by CodeForBuffalo</a>
          <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
        </div>
      </div>
    </div>
  </div>
</section>
