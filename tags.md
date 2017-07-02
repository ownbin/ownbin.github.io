---
layout: page
title: Tags
banner_image: sample-banner-image-3.jpg
---

<div>
  {% for tag in site.tags %} 
    <h5>{{ tag[0] }}</h5>
    <ul>
    {% for post in tag[1] %} 
      <li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}
    </ul>
  {% endfor %}
</div>