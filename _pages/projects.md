---
layout: page
title: Work With Me
permalink: /research/
nav: true
nav_order: 2
display_categories: [Freelance Rates, Weekly Availability]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  <!-- Generate cards for each project -->
  {% if category == "Freelance Rates" %}
  <div class="container">
    <div class="row row-cols-1">
       <div class="flex"><h3 class="d-inline-flex">Standard Rate</h3><span>: 40£/hr</span></div>
       <div class="flex"><h3 class="d-inline-flex">Sliding Scale</h3><span>: Feel free to <a href="/cv/#basics-1" target="_blank">contact me</a> with details for more info!</span></div>
    </div>
  </div>
  {% else if category == "Weekly Availability" %}
  <div class="container">
    <div class="d-flex justify-content-between">
       <p>Free two days a week to spelunk in the archives.</p>
       <img class="cats" src="/assets/img/cats.png" alt="Cat Illustration">
    </div>
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
