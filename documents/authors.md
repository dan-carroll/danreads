---
layout: default
title: Authors
---

{% for author in site.authors %}
  <h2>
    <a href="{{ author.url | relative_url }}">
      {{ author.name }} - {{ author.genre }} Writer
	</a>
  </h2>	
  <p>{{ author.content | markdownify }}</p>
{% endfor %}
