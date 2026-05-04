---
layout: project
title: "PowGenAUS: Interactive Geospatial Dashboard for Australian Power Generation"
category: "WebGIS & Application Development"
summary: "A Streamlit dashboard for exploring Australian power stations, generation patterns, fuel types and state-level capacity using Python, GeoPandas, Folium and Plotly."
tools: ["Python", "Streamlit", "GeoPandas", "Folium", "Plotly", "Pandas", "Shapely"]
status: "Completed course project"
period: "Application Development Course"
featured: true
image: "/assets/img/projects/powgenaus-home.jpg"
gallery:
  - image: "/assets/img/projects/powgenaus-home.jpg"
    caption: "Dashboard overview with filters and key summary indicators."
  - image: "/assets/img/projects/powgenaus-map.jpg"
    caption: "Map explorer with choropleth mapping and power-station markers."
  - image: "/assets/img/projects/powgenaus-charts.jpg"
    caption: "Interactive charts for fuel type, state comparison and generation patterns."
  - image: "/assets/img/projects/powgenaus-data.jpg"
    caption: "Data inspection and downloadable tables for filtered records."
links:
  - label: "Live Streamlit application"
    url: "https://powgenaus-dashboard.streamlit.app"
  - label: "GitHub repository"
    url: "https://github.com/euphoricking/powgenaus-power-generation-dashboard"
---

## Overview

PowGenAUS is an interactive Python dashboard for exploring power generation and power station capacity across Australia. It was developed as a software development project within the MSc Applied Geoinformatics programme and demonstrates practical geospatial processing, dashboard development and exploratory data visualisation.

## Problem and Motivation

Energy infrastructure data can be difficult to interpret when presented only as large tables. This project transforms power-plant records into an interactive geospatial dashboard that helps users explore where power stations are located, which fuel types dominate, how generation changes over time and how capacity differs across Australian states and territories.

## Data and Processing

The application uses the Global Power Plant Database filtered to Australian records and combines it with Australian state boundary GeoJSON data. Python is used to clean the tabular dataset, convert coordinates into geospatial point features and spatially join power stations to state polygons.

## Application Features

The dashboard includes sidebar filters for year, fuel type, state, minimum capacity and station or owner name. It provides summary indicators, a state-level choropleth layer, optional clustered power-station markers, detailed popups, interactive Plotly charts, fuel and state summaries, top-station rankings and CSV download options.

## Skills Demonstrated

This project demonstrates Python software development, Streamlit interface design, geospatial processing with GeoPandas, interactive WebGIS mapping with Folium, marker clustering, popup design, Pandas-based aggregation, Plotly charting and GitHub-ready project organisation.
