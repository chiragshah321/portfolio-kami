---
layout: page
title: Projects
permalink: /projects/
feature-img: "img/color.png"
---

  <div class="work">
    <h2>My Work</h2>
    {% for project in site.portfolio limit:10 %}
    <div class="project">
      <div class="project-thumb">
        <a href="{{ project.url | prepend: site.baseurl }}">
          <img src="{{ project.thumbnail-path }}" alt="{{ project.title }}"/>
        </a>
      </div>
      <div class="project-description">
        <a href="{{ project.url | prepend: site.baseurl }}"><strong>{{ project.title }}</strong></a>
        <p>{{ project.short-description }}</p>
      </div>
    </div>
    {% endfor %}
  </div>

