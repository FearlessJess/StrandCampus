---
title: About
layout: index
permalink: /about/
---

 
<br/><br/><br/><br/><br/><br/><br/><br/>
<p id="about">A museum about the history of buildings in King's Strand campus, the biggest campus at King's in the heart of London, targeting at all people who are interested in King's College London. You can find information about Strand Building, King's Building, Somerset House East Wing, Bush House, Maughan Library, Roman Bath and Tube Station here to understand the general history and hidden facts behind the scene.</p>

<p id="about">Created by:
{% assign authors_alphabetical = site.data.authors | sort: "name" %}
{% for author in authors_alphabetical %}
  <a href = "{{ author.homepage }}">{{ author.name }}</a>
{% endfor %}
</p>

<br/><br/><br/><br/><br/>

 <div class = "footer">
            <ul id= "footer_text">
                <p>Created with <a href = "https://jekyllrb.com/">Jekyll</a> for learning purposes by KCL students in 2021</p>
            </ul>
        </div>