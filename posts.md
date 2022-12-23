---
layout: page
title: Articles
date: 2022-12-23
---



<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <div class="image">
        <img src="{{ post.picture }}"/>
      </div>
      <div class="entry">
        <h2 class="project"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
          {{ post.description }}
      </div>
    </article>
  {% endfor %}
</div>


