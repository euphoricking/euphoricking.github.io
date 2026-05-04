---
layout: default
title: Home
---

<section class="hero enhanced-hero">
  <div class="container hero-grid">
    <div class="hero-copy">
      <p class="eyebrow">GIS · Spatial Data Science · Business Intelligence</p>
      <h1>Ekata Leo Oni</h1>
      <p class="hero-subtitle">
        MSc Applied Geoinformatics | GIS, Spatial Databases, WebGIS, GeoAI & Data Engineering
      </p>
      <p class="lead">
        I am an MSc Applied Geoinformatics student and Business Intelligence Developer
        with interests in spatial analysis, WebGIS, spatial databases, geospatial machine learning,
        SQL reporting, and data engineering.
      </p>

      <div class="button-row">
        <a class="button primary" href="{{ '/portfolio/' | relative_url }}">View Portfolio</a>
        <a class="button secondary" href="{{ '/thesis/' | relative_url }}">View MSc Thesis</a>
        <a class="button ghost" href="{{ '/cv/' | relative_url }}">View CV</a>
      </div>

      <div class="tag-row hero-tags">
        <span class="tag">GIS</span>
        <span class="tag">Spatial Databases</span>
        <span class="tag">WebGIS</span>
        <span class="tag">GeoAI</span>
        <span class="tag">BI</span>
        <span class="tag">Data Engineering</span>
      </div>
    </div>

    <div class="profile-panel">
      <div class="profile-card">
        <div class="profile-image-wrap">
          <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile placeholder" class="profile-image">
        </div>
        <div class="profile-info">
          <p class="profile-kicker">Personal ePortfolio</p>
          <h2>Applied Geoinformatics Portfolio</h2>
          <p>
            A curated collection of MSc projects, thesis research, WebGIS applications,
            spatial database work, and data engineering outputs.
          </p>
        </div>
      </div>

      <div class="floating-stat stat-one">
        <strong>6+</strong>
        <span>Portfolio project areas</span>
      </div>
      <div class="floating-stat stat-two">
        <strong>GIS + BI</strong>
        <span>Spatial and business data</span>
      </div>
    </div>
  </div>
</section>

<section class="section light tech-section">
  <div class="container">
    <div class="section-heading">
      <p class="eyebrow">Technologies & Tools</p>
      <h2>Technologies I work with</h2>
      <p>
        A selection of tools and technologies I use across GIS, spatial databases,
        WebGIS, data analysis, cloud data engineering, and business intelligence projects.
      </p>
    </div>

    <div class="tech-grid">
      <div class="tech-card"><span class="tech-icon">Py</span><h3>Python</h3><p>Automation, analysis and geospatial workflows</p></div>
      <div class="tech-card"><span class="tech-icon">SQL</span><h3>SQL</h3><p>Data extraction, transformation and reporting</p></div>
      <div class="tech-card"><span class="tech-icon">PG</span><h3>PostGIS</h3><p>Spatial database design and queries</p></div>
      <div class="tech-card"><span class="tech-icon">Q</span><h3>QGIS</h3><p>Spatial analysis and cartography</p></div>
      <div class="tech-card"><span class="tech-icon">AG</span><h3>ArcGIS Pro</h3><p>Mapping, spatial processing and visualization</p></div>
      <div class="tech-card"><span class="tech-icon">Lf</span><h3>Leaflet</h3><p>Interactive web mapping and dashboards</p></div>
      <div class="tech-card"><span class="tech-icon">GP</span><h3>GeoPandas</h3><p>Spatial data handling in Python</p></div>
      <div class="tech-card"><span class="tech-icon">ML</span><h3>Scikit-learn</h3><p>Machine learning and predictive modelling</p></div>
      <div class="tech-card"><span class="tech-icon">BI</span><h3>Power BI</h3><p>Business intelligence dashboards</p></div>
      <div class="tech-card"><span class="tech-icon">BQ</span><h3>BigQuery</h3><p>Cloud analytics and warehousing</p></div>
      <div class="tech-card"><span class="tech-icon">GH</span><h3>GitHub</h3><p>Version control and portfolio publishing</p></div>
      <div class="tech-card"><span class="tech-icon">Nb</span><h3>Jupyter</h3><p>Research notebooks and analysis workflows</p></div>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="section-heading">
      <p class="eyebrow">Portfolio Highlights</p>
      <h2>Selected geospatial and data projects</h2>
      <p>
        A curated selection of academic, technical, and professional projects from my MSc Applied
        Geoinformatics journey and data engineering practice.
      </p>
    </div>

    <div class="project-grid">
      {% assign featured_projects = site.projects | where: "featured", true %}
      {% for project in featured_projects limit:3 %}
        {% include project-card.html project=project %}
      {% endfor %}
    </div>
  </div>
</section>

<section class="section light">
  <div class="container split">
    <div>
      <p class="eyebrow">What I Work On</p>
      <h2>Applied geoinformatics with a practical data engineering mindset</h2>
      <p>
        My work connects GIScience concepts with practical implementation: spatial data modelling,
        reproducible Python workflows, interactive dashboards, SQL-based reporting, and WebGIS
        applications for communication and decision support.
      </p>
    </div>

    <div class="feature-list">
      <div class="feature-item">
        <h3>Spatial Analysis</h3>
        <p>Spatial joins, proximity analysis, KDE, hot spot analysis, spatial statistics, and modelling.</p>
      </div>
      <div class="feature-item">
        <h3>Spatial Databases</h3>
        <p>PostGIS, GeoPackage, SQL Server, ERD design, indexing, views, and spatial queries.</p>
      </div>
      <div class="feature-item">
        <h3>WebGIS & Dashboards</h3>
        <p>Leaflet, Folium, Chart.js, GeoJSON, ArcGIS dashboards, and interactive visualization.</p>
      </div>
    </div>
  </div>
</section>
