---
layout: project
title: "MSc Thesis: Crime Hotspot Prediction Using Geospatial Data Mining"
category: "MSc Thesis & Research"
summary: "A geospatial machine learning study that predicts crime hotspots across Chicago community areas using historical crime records, livability indicators, accessibility measures, spatial lag variables and supervised learning models."
tools: ["Python", "GeoPandas", "OSMnx", "Scikit-learn", "PySAL", "QGIS", "Folium", "GeoAI"]
status: "MSc thesis project"
period: "2025-2026"
featured: true
image: "/assets/img/projects/thesis-hotspot-comparison.jpg"
gallery:
  - image: "/assets/img/projects/thesis-hotspot-comparison.jpg"
    caption: "Observed and predicted hotspot comparison for Chicago community areas."
  - image: "/assets/img/projects/thesis-livability-maps.jpg"
    caption: "Livability and accessibility indicators used as spatial context variables."
  - image: "/assets/img/projects/thesis-title.jpg"
    caption: "Thesis title page and academic context."
links:
  - label: "Download thesis report"
    url: "/assets/files/projects/msc-thesis-report.pdf"
---

## Overview

This MSc thesis investigates how geospatial data mining and predictive analysis can support crime hotspot prediction in Chicago. The study moves beyond a purely historical crime-count approach by integrating spatial context, livability measures, amenity accessibility and neighbourhood relationships into the modelling workflow.

## Problem and Motivation

Many crime prediction workflows depend heavily on previous crime occurrence. Although historical crime is an important predictor, it does not fully explain the urban conditions that may contribute to persistent or emerging hotspots. This project addresses that limitation by combining crime records with spatially derived indicators from OpenStreetMap amenities and Chicago community-area geography.

## Data and Features

The analysis uses historical Chicago crime records aggregated to community areas, OpenStreetMap amenity layers, community boundary data and derived spatial features. Two complementary livability measures were developed: a **Unified Livability Index** based on amenity density and diversity, and a **Distance-Based Livability Index** based on accessibility to services using pedestrian street-distance concepts. Temporal crime lag variables and a Queen-contiguity spatial lag feature were also included.

## Methods

The workflow combines spatial preprocessing, feature engineering, spatial statistics and supervised machine learning. Global Moran's I was used to examine spatial clustering. Logistic Regression, Random Forest and XGBoost models were trained and compared using a time-aware evaluation approach, with later years reserved for testing to reflect a more realistic prediction setting.

## Results and Reflection

The enhanced Random Forest model performed best overall and showed that historical crime patterns remained the strongest predictors. However, spatial lag and livability variables added explanatory value, especially when density-based and accessibility-based indicators were used together. The project strengthened my ability to connect GIScience, spatial statistics, GeoAI and urban safety analysis into a coherent research workflow.
