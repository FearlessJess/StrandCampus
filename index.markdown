---
title: Buildings at Strand Campus, King's College London
layout: index
---


<!-- 首页预览部分 -->
{% for building in site.buildings %}
<p>{{ building. image-url1 }}</p> <!-- 首页头图 -->
<p>{{ building.title }}</p>
{% endfor %}

