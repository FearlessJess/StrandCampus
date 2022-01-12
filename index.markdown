---
title: Buildings at Strand Campus, King's College London
layout: index
---
 
 <br /> <br /> <br /> <br />

<!-- introduction -->
<div id= "introduction">
<p>MORE THAN A CAMPUS: PAST AND PRESENT </p><br />            
<p>Uncover the hidden London!<br><br>
Start your exploration in the Strand campus, King's College London. </p>
</div>

<!-- preview part -->
<div id = "wrapper">
<div id = "gallery">
{% assign sorted_buildings = site.buildings | sort: "title" %}
    {% for building in sorted_buildings %}
      {% assign author = site.data.authors | find: "name", building.creator %}       
<div class = "grid_cell">
                    <a href = "{{ building.url | relative_url }}"><img src="{{ building.image-url1 }}" title="{{ building.title }}" class="gallery_thumb"></a>
                    <p class = "caption"><a href = "{{ building.url | relative_url }}">{{ building.title }}</a> by <a href = "{{ author.homepage }}">{{ building.creator }}</a></p>                    </div>
                    {% endfor %}
                    <br/>
                    </div>
   

<!-- footer -->       
<div class = "footer">
<ul id= "footer_text">
<br/><br/>
<p>Created with <a href = "https://jekyllrb.com/">Jekyll</a> for learning purposes by KCL students in 2021</p><br/><br/>
</ul>
</div> 
</div>
                    

