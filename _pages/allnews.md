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

<a href="https://twitter.com/twitter?ref_src=twsrc%5Etfw" class="twitter-follow-button" data-show-count="false">Follow @twitter</a><script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
