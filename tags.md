---
layout: page
title: Tags
banner_image: sample-banner-image-3.jpg
---

<div>
  <!-- tag cloud -->
  {% for tag in site.tags %}
    <a href="{{ tag[0] | prepend: '/tags/#' | prepend: site.baseurl }}">{{ tag[0] }} ({{ tag[1].length }}) </a>
  {% endfor %}
  <hr>
  
  <!-- tag post -->
  {% for tag in site.tags %} 
    <h5 id="{{ tag[0] }}">{{ tag[0] }}</h5>
    <ul>
    {% for post in tag[1] %} 
      <li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}
    </ul>
  {% endfor %}
</div>