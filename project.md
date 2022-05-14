---
layout: project
title: Projects
description: this is the gallery page
baseurl: project
order: 3
---

{% include nav.html %}

{% for block in site.data.project.list %}
  <div class="projects">
    <div class="project">
      <div class="pic">
         <img src="{{block.image}}" alt="{{block.image-alt}}">
      </div>
    <div class="content">
      <h3 class="title">{{block.title}}</h3>
      <p>{{block.list-content}}</p>
    </div>
  </div>
</div>
{% endfor %}



KR