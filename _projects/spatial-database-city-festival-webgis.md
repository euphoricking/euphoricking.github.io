---
layout: project
title: "Spatial Database Backend for a City Festival WebGIS"
category: "Spatial Databases & SDI"
summary: "A PostgreSQL/PostGIS spatial database backend for managing festival locations, events, attractions, facilities and zones, with spatial indexes, views and dynamic spatial queries."
tools: ["PostgreSQL", "PostGIS", "SQL", "QGIS", "ArcGIS Pro", "ERD", "Spatial Indexing"]
status: "Completed course project"
period: "Spatial Database Course"
featured: false
image: "/assets/img/projects/spatial-db-workflow.jpg"
gallery:
  - image: "/assets/img/projects/spatial-db-workflow.jpg"
    caption: "Implementation workflow showing SQL table creation and data insertion."
  - image: "/assets/img/projects/spatial-db-report.jpg"
    caption: "Project documentation describing the database backend and use case."
links:
  - label: "Download documentation"
    url: "/assets/files/projects/spatial-database-documentation.pdf"
  - label: "Download workflow report"
    url: "/assets/files/projects/spatial-database-workflow.pdf"
  - label: "Download SQL scripts"
    url: "/assets/files/projects/spatial-database-sql.zip"
---

## Overview

This project developed a spatial database backend for a WebGIS-based city festival management scenario. The database was designed in PostgreSQL with PostGIS to manage festival locations, events, attractions, public facilities and zones.

## Problem and Motivation

A city festival involves many spatially distributed assets: stages, attractions, toilets, first-aid points, security posts, food booths and event zones. A static table or paper-based approach is not enough for efficient planning and visitor support. A spatial database provides a structured backend for location-based queries, GIS visualisation and WebGIS integration.

## Database Design

The database, named `festival_db`, uses a normalized relational-spatial structure. Core entities include `festival_info`, `facility`, `event`, `attraction` and `zone`. Spatial data are stored using PostGIS geometry types such as points and polygons with SRID 4326.

## Spatial Queries and Optimisation

The implementation includes spatial indexes, a unified spatial-entities view and dynamic spatial queries. Example queries include finding facilities within 500 metres of a point, identifying nearby events or attractions, finding the nearest facility, counting events or facilities inside each zone and retrieving security-related facilities.

## Reflection

This project strengthened my understanding of spatial database modelling, SQL implementation, spatial indexing and the relationship between a PostGIS backend and GIS/WebGIS frontends. It also improved my ability to document technical database workflows clearly.
