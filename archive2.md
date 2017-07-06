---
layout: page
title: Archive
banner_image: sample-banner-image-3.jpg
---

<div class="tags-expo">
<div class="tags-expo-section">

<ul class="tags-expo-posts">
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
    <h3>{{ y }}</h3>
  {% endif %}

  <a class="post-title" href="{{ site.baseurl }}{{ post.url }}">
    <li>
    {{ post.title }}
    <small class="post-date">{{ post.date | date_to_string }}</small>
    </li>
  </a>
{% endfor %}
</ul>

</div>
</div>