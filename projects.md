---
layout: page
title: Projects
date: 2022-12-23
---


<div class="posts">
  {% for project in site.projects %}
    <article class="post">
      <div class="image">
        <img src="{{ project.picture }}"/>
      </div>
      <div class="entry">
        <h2 class="project"><a href="{{ site.baseurl }}{{ project.url }}">{{ project.title }}</a></h2>
          {{ project.description }}
      </div>
    </article>
  {% endfor %}
</div>

