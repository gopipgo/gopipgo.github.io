---
layout: page
title: Reviews
---

{% for reviews in site.reviews %}

<a href="{{ reviews.url | prepend: site.baseurl }}">
  <h2>{{ reviews.title }}</h2>
</a>

<p class="post-excerpt">{{ reviews.description | truncate: 160 }}</p>

{% endfor %} 