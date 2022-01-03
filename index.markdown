---
title: Buildings at Strand Campus, King's College London
layout: index
---
 
 <br /> <br />
<div id= "introduction">
<p>This is a simple historical archive about the buildings of King's Strand Campus, the biggest campus at King's in the heart of London. Brief history stories, architecture style and current function about these building can be found here, a good site for anyone who is interested in King's.</p>
</div>
 <br />


<div id = "gallery">
  {% assign sorted_buildings = site.buildings | sort: "title" %}
  {% for building in site.buildings %}
    {% assign author = site.data.authors | find: "name", building.creator %}

    <div class = "grid_cell">
        <a href = "{{ building.url | relative_url }}"><img src="{{ building.image-url1 }}" class="gallery_thumb"></a>
        <p class = "caption"><a href = "{{ building.url | relative_url }}">{{ building.title }}</a> by <a href = "{{ author.homepage }}">{{ building.creator }}</a></p>
        
        <!-- 加了每个版块的作者 -->
    </div>
  {% endfor %}
</div>
