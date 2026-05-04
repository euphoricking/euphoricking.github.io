---
layout: default
title: Portfolio
permalink: /portfolio/
---

<section class="page-hero compact">
  <div class="container">
    <p class="eyebrow">Portfolio</p>
    <h1>Selected projects in geoinformatics, WebGIS, spatial databases, SDI and data engineering.</h1>
    <p class="lead">
      This portfolio documents selected academic and technical work developed during my MSc Applied
      Geoinformatics studies and professional data practice.
    </p>
  </div>
</section>

<section class="section">
  <div class="container">
    {% assign categories = "MSc Thesis & Research|WebGIS & Application Development|Spatial Databases & SDI|Data Engineering & BI" | split: "|" %}

    {% for category in categories %}
    <div class="category-block">
      <div class="section-heading left">
        <p class="eyebrow">{{ category }}</p>
        <h2>{{ category }}</h2>
      </div>

      <div class="project-grid">
        {% assign filtered = site.projects | where: "category", category %}
        {% for project in filtered %}
          {% include project-card.html project=project %}
        {% endfor %}
      </div>
    </div>
    {% endfor %}
  </div>
</section>
