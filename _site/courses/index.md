---
title: Personal Links
layout: page
eleventyNavigation:
  key: courses
  parent: main
---

# {{title}}

<div class="container mt-4">
  <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3">
  {% for course in courses %}
  <div class="col mb-4">
    <div class="card h-100" >
      <img src="{{ course.thumbnail | safe }}" alt="{{ course.title | safe }} image" class="card-img-top">
      <div class="card-body">
        <h5 class="card-title my-0"></h5>
        <time class="item-date small d-block text-muted mb-2" datetime="{{ course.date | safe }}">{{ course.date | courseDate }}</time>
        <p class="card-text"></p>
        <a href="{{ course.url | url }}" class="btn btn-secondary stretched-link" target="_blank">{{ course.title | safe }}</a>
      </div>
    </div>
  </div>
  {% endfor %}

  </div>