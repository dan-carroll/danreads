---
layout: default
title: Authors
description: Some of my favorite authors.
---

  <div class="row">
    <div class="col">
		<img src="/assets/img/authors/Authors_collage_banner.jpg" alt="authors collage" img-fluid width="100%">
    </div>
  </div>
  <div class="row">
  
  {% for author in site.authors %}

    <div class="col">
      <div class="card my-3 mx-auto" style="width: 18rem;">
		<img class="card-img-top mx-auto" src="{{ author.photo }}" alt="{{ author.name }} photo" style="max-width: 80%;height:auto;">
		<div class="card-body">
		  <h2 class="card-title">{{ author.title }}</h2>
		  <h5 class="card-subtitle">{{ author.genre }} Writer</h5>
			<p class="card-text">{{ author.intro | markdownify }}</p>
			<a href="{{ author.url | relative_url }}" class="btn btn-primary">Author's Page</a>
		</div>
	  </div>
    </div>
	
  {% endfor %}	
    
  </div>