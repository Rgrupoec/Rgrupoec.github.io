---
layout: page
title: Publicaciones
subtitle: Temario de publicaciones
published: true
comments: true
---
  
<ul class="tag-box inline">
{% assign tags_list = site.publicaciones %}  
  {% if tags_list.first[0] == null %}
    {% for tag in tags_list %} 
      <li><a href="#{{ tag }}">{{ tag | capitalize }} <span>{{ site.tags[tag].size }}</span></a></li>
    {% endfor %}
  {% else %}
    {% for tag in tags_list %} 
      <li><a href="#{{ tag[0] }}">{{ tag[0] | capitalize }} <span>{{ tag[1].size }}</span></a></li>
    {% endfor %}
  {% endif %}
{% assign tags_list = nil %}
</ul>

{% for tag in site.categories %} 
  <h2 id="{{ tag[0] }}">{{ tag[0] | capitalize }}</h2>
  <ul class="post-list">
    {% assign pages_list = tag[1] %}  
    {% for post in pages_list %}
      {% if post.title != null %}
      {% if group == null or group == post.group %}
      <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
      {% endif %}
      {% endif %}
    {% endfor %}
    {% assign pages_list = nil %}
    {% assign group = nil %}
  </ul>
{% endfor %}
