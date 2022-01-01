---
title: Buildings at Strand Campus, King's College London
layout: index
---
 
 <br />
<div id= "introduction">
This is a simple historical archive about the buildings of King's Strand Campus, the biggest campus at King's in the heart of London. Brief history stories, architecture style and current function about these building can be found here, a good site for anyone who is interested in King's.  
</div>
 <br />


<div id = "gallery">
  {% assign sorted_buildings = site.buildings | sort: "title" %}
{% for building in site.buildings %}
   <div class = "grid_cell">
      <a href = "{{ building.url | relative_url }}"><img src="{{ building.image-url1 }}" class="gallery_thumb"></a>
      <p class = "caption"><a href = "{{ building.url | relative_url }}">{{ building.title }}</a> </p>
    </div>
  {% endfor %}
</div>
