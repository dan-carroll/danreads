---
layout: default
title: Authors
description: Some of my favorite authors.
---

  <div class="row">
    <div class="col">
		<img src="/assets/img/authors/Authors_collage_banner.jpg" alt="authors collage" class="img-fluid" width="100%">
		
	  <h1 class="mt-1 text-center text-primary display-2">Some of My Favorite Authors</h1>
	  <h4 class="text-muted display-4 pl-5 pb-3">And Others I Have Read</h4>
    </div>
  </div>
  <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3">
  
  {% for author in site.authors %}

	<div class="col mb-4 mx-auto">
        <div class="card mx-3" style="width: 18rem;">
		  <img class="card-img-top mx-auto" src="{{ author.photo }}" alt="{{ author.name }} photo" style="max-width: 80%;height:auto;">
		  <div class="card-body">
		    <h2 class="card-title">{{ author.title }}</h2>
		    <h5 class="card-subtitle text-muted">{{ author.genre }} Writer</h5>
			  <p class="card-text">{{ author.intro | markdownify }}</p>
			  <a href="{{ author.url | relative_url }}" class="btn btn-primary">Author's Page</a>
		  </div>
		</div>
    </div>
	
  {% endfor %}	
    
  </div>