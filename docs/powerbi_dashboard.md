# Blinkit Sales Analysis – Power BI Dashboard Documentation

## Overview

This document describes the **design, structure, and analytical logic** of the Power BI dashboard created for the **Blinkit Sales Performance Analysis** project.

The dashboard serves as the visualization layer of the analytics pipeline, enabling interactive exploration of key performance indicators (KPIs) and sales trends across products, outlets, and locations.

---

## Dashboard Objectives

The Power BI dashboard was designed to:

- Present key sales KPIs in a concise and intuitive manner
- Enable comparison across product categories and outlet attributes
- Support interactive filtering and drill-down analysis
- Provide business-ready insights for decision-making

---

## Key Performance Indicators (KPIs)

The dashboard highlights the following KPIs:

- **Total Sales** – Overall revenue generated
- **Average Sales** – Average revenue per transaction
- **Number of Items Sold** – Total items sold
- **Average Rating** – Customer satisfaction indicator

These KPIs are consistent with metrics calculated using SQL and validated using Python.

---

## Visual Components

The dashboard includes multiple visual elements to support analysis:

### KPI Cards
- Display overall summary metrics
- Provide an at-a-glance view of business performance

### Bar Charts
- Total sales by item type
- Total sales by fat content

### Donut Charts
- Percentage contribution of sales by outlet size

### Column and Line Charts
- Sales trends by outlet establishment year
- Comparison of outlet performance over time

### Tables
- Outlet-type level performance comparison
- Consolidated view of all KPIs by outlet type

---

## Outlet-Level Analysis

The dashboard enables outlet-level insights across multiple dimensions:

- **Outlet Size:** Small, Medium, Large
- **Outlet Location Type:** Tier-based geographic classification
- **Outlet Type:** Grocery store, supermarket variants

This segmentation allows comparison of performance patterns across different outlet configurations.

---

## Interactivity and Filters

Interactive slicers are implemented to allow filtering by:

- Outlet location type
- Outlet size
- Item type
- Fat content

These filters enable dynamic exploration of data and support ad-hoc analysis without modifying the underlying dataset.

---

## Data Model and Measures

- The Power BI data model is based on a cleaned and standardized dataset.
- Relationships are validated to ensure accurate aggregation.
- Calculated measures are used to maintain consistency with SQL-derived KPIs.
- Aggregations are designed to avoid duplication and overcounting.

---

## Business Insights Enabled

The dashboard supports identification of:

- High-performing and underperforming product categories
- Revenue contribution by outlet size and location
- Sales trends across outlet establishment years
- Relationships between customer ratings and sales performance

---

## Usage in This Project

In this project, the Power BI dashboard is used to:

- Visualize KPIs computed through SQL
- Validate analytical findings from Python
- Present insights in an interactive and business-friendly format

---

## Conclusion

The Power BI dashboard acts as the final presentation layer of the Blinkit Sales Analysis project, translating structured analytical logic into interactive visuals that support data-driven decision-making.
