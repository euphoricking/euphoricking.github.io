---
layout: default
title: MSc Thesis
permalink: /thesis/
---

<section class="page-hero">
  <div class="container">
    <p class="eyebrow">MSc Thesis</p>
    <h1>Crime Hotspot Prediction Using Geospatial Data Mining and Predictive Analysis</h1>
    <p class="lead">
      A geospatial machine learning study integrating historical crime records, livability indicators,
      accessibility measures and spatial statistics for crime hotspot prediction across Chicago community areas.
    </p>
    <div class="button-row">
      <a class="button primary" href="{{ '/portfolio/msc-thesis-crime-hotspot-prediction/' | relative_url }}">Read full project page</a>
      <a class="button ghost" href="{{ '/assets/files/projects/msc-thesis-report.pdf' | relative_url }}">Download thesis report</a>
    </div>
  </div>
</section>

<section class="section">
  <div class="container content-grid">
    <article class="content-card">
      <h2>Thesis Overview</h2>
      <p>
        This thesis develops a spatially informed machine learning workflow for predicting crime hotspots in Chicago.
        It combines historical crime data with spatially derived livability and accessibility indicators from OpenStreetMap,
        temporal crime lag variables and a spatial lag feature based on neighbouring community areas.
      </p>

      <h2>Research Aim</h2>
      <p>
        The aim is to evaluate whether crime hotspot prediction can be improved when historical crime patterns are combined
        with urban spatial context, amenity accessibility and spatial dependence.
      </p>

      <h2>Methodological Workflow</h2>
      <ol class="timeline">
        <li><strong>Data acquisition:</strong> Chicago crime records, community boundaries and OpenStreetMap amenity data.</li>
        <li><strong>Preprocessing:</strong> data cleaning, temporal extraction, spatial joins and community-level aggregation.</li>
        <li><strong>Feature engineering:</strong> Unified Livability Index, Distance-Based Livability Index, temporal lag variables and spatial lag features.</li>
        <li><strong>Spatial analysis:</strong> spatial clustering assessment using Moran's I and hotspot interpretation.</li>
        <li><strong>Modelling:</strong> Logistic Regression, Random Forest and XGBoost classification models.</li>
        <li><strong>Evaluation:</strong> model comparison, feature importance and spatial interpretation of prediction results.</li>
      </ol>
    </article>

    <aside class="content-card accent-card">
      <h2>Tools & Methods</h2>
      <div class="tag-row">
        <span class="tag">Python</span>
        <span class="tag">GeoPandas</span>
        <span class="tag">OSMnx</span>
        <span class="tag">Scikit-learn</span>
        <span class="tag">PySAL</span>
        <span class="tag">QGIS</span>
        <span class="tag">Folium</span>
        <span class="tag">Spatial Statistics</span>
      </div>

      <h2>Core Outputs</h2>
      <ul class="clean-list">
        <li>Crime hotspot prediction maps</li>
        <li>Unified and Distance-Based Livability Index indicators</li>
        <li>Spatial lag and temporal lag features</li>
        <li>Model comparison and feature importance interpretation</li>
      </ul>
    </aside>
  </div>
</section>

<section class="section light">
  <div class="container">
    <div class="section-heading">
      <p class="eyebrow">Thesis Visuals</p>
      <h2>Selected thesis outputs</h2>
    </div>
    <div class="visual-grid image-visual-grid">
      <img src="{{ '/assets/img/projects/thesis-hotspot-comparison.jpg' | relative_url }}" alt="Chicago predicted and observed hotspot comparison">
      <img src="{{ '/assets/img/projects/thesis-livability-maps.jpg' | relative_url }}" alt="Livability and accessibility maps">
    </div>
  </div>
</section>
