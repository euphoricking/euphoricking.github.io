---
layout: project
title: "BlockPulse: Cloud-Native Cryptocurrency Data Engineering Pipeline"
category: "Data Engineering & BI"
summary: "A GCP-based daily ETL pipeline that ingests cryptocurrency market data from CoinGecko, stores raw snapshots in GCS, models the data in BigQuery and powers Looker Studio analytics."
tools: ["Python", "GCP", "Cloud Composer", "Airflow", "GCS", "BigQuery", "Looker Studio", "CoinGecko API"]
status: "Completed capstone project"
period: "Data Engineering"
featured: true
image: "/assets/img/projects/blockpulse-dashboard.jpg"
gallery:
  - image: "/assets/img/projects/blockpulse-dashboard.jpg"
    caption: "Looker Studio dashboard showing market cap, volume, market share and coin performance."
  - image: "/assets/img/projects/blockpulse-architecture.jpg"
    caption: "Pipeline architecture from CoinGecko API ingestion to warehouse and dashboard analytics."
links:
  - label: "Live Looker Studio dashboard"
    url: "https://lookerstudio.google.com/s/mcn2g1qssxA"
  - label: "GitHub repository"
    url: "https://github.com/euphoricking/blockpulse"
  - label: "Download presentation"
    url: "/assets/files/projects/blockpulse-presentation.pdf"
  - label: "Download dashboard PDF"
    url: "/assets/files/projects/blockpulse-dashboard.pdf"
---

## Overview

BlockPulse is a cloud-native data engineering project for daily cryptocurrency market intelligence. It captures market snapshots from the CoinGecko API, stores raw files in Google Cloud Storage, loads and transforms the data in BigQuery and powers an interactive Looker Studio dashboard.

## Objective and Use Case

The goal was to automate the collection and preparation of cryptocurrency market data so that analysts can track prices, market capitalisation, trading volume and market ranking without manual data gathering. The project converts raw API responses into a clean analytical warehouse suitable for dashboards and future analytical extensions.

## Pipeline Architecture

The pipeline uses Python scripts to call the CoinGecko API, normalise JSON responses and produce structured snapshot files. Airflow in Cloud Composer orchestrates the daily workflow. Raw data lands in GCS, while BigQuery stores staging, dimension and fact tables.

## Dimensional Model

The warehouse follows a star-schema design. The `crypto_market_snapshot_fact` table stores daily metrics per coin, including price, volume, market cap, rank and daily change. The `crypto_asset_dim` table stores coin metadata, while `date_dim` provides calendar attributes for each snapshot date.

## Dashboard and Analytics

The Looker Studio dashboard includes market snapshot visuals, coin performance trends, market-share views, rank changes, daily percentage-change heatmaps and comparative charts for size and liquidity. Interactive filters allow users to select date ranges and coins.

## Reflection

This project demonstrates my ability to design a full data pipeline from API ingestion to cloud storage, warehouse modelling, orchestration and dashboard delivery. It also connects my data engineering background with analytical storytelling and business intelligence.
