---
title: Buildings at Strand Campus, King's College London
layout: index
---
 
 <br />
<div id= "introduction">
This is a simple historical archive about the buildings in strand campus, King's College London. 
Brief history stories, architecture style and current function about these building can be found here, giving you a general understanding about King's strand campus.  
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
