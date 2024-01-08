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
