# Blinkit Sales Performance Analysis  
**SQL | Python | Power BI**

## Overview

This project presents a comprehensive **sales performance analysis for Blinkit**, focusing on revenue trends, customer satisfaction, and outlet-level performance.  
The analysis integrates **SQL for data querying**, **Python for exploratory analysis**, and **Power BI for visualization** to generate actionable business insights.

The objective of this project is to evaluate key performance indicators (KPIs) and identify opportunities for optimization across products, outlets, and regions.

---

## Business Objective

To analyze Blinkit’s sales data in order to:
- Measure overall sales performance
- Evaluate customer satisfaction using ratings
- Understand outlet-level and location-based performance
- Support data-driven decision-making through KPIs and dashboards

---

## Dataset Overview

The dataset contains structured retail data, including:
- Item attributes and categories
- Fat content classification
- Outlet characteristics (size, type, location, establishment year)
- Sales values and customer ratings

---

## Technology Stack

- **SQL:** Data cleaning, aggregation, KPI computation
- **Python:** Exploratory data analysis and validation
- **Power BI:** Interactive dashboard and visualization
- **Domain:** Retail & E-commerce Analytics

---

## Data Preparation and Cleaning

Data quality improvements were applied before analysis:
- Standardized `Item_Fat_Content` values  
  (e.g., `LF`, `low fat` → `Low Fat`; `reg` → `Regular`)
- Ensured categorical consistency for accurate grouping
- Validated numeric and rating fields for KPI calculations

These steps improved consistency and reliability of analytical outputs.

---

## Key Performance Indicators (KPIs)

The following KPIs were calculated:

- **Total Sales** – Overall revenue generated
- **Average Sales** – Average revenue per transaction
- **Number of Items** – Total count of items sold
- **Average Rating** – Customer satisfaction indicator

---

## Analytical Breakdown

### Total Sales by Fat Content
- Compared sales contribution of `Low Fat` and `Regular` items
- Evaluated associated KPIs such as average sales and ratings

### Total Sales by Item Type
- Identified high-performing product categories
- Ranked item types based on total sales

### Fat Content by Outlet for Total Sales
- Analyzed outlet-level sales segmented by fat content
- Used pivot-based aggregation for comparison

### Total Sales by Outlet Establishment Year
- Evaluated sales trends across outlet establishment years

### Percentage of Sales by Outlet Size
- Measured revenue contribution of small, medium, and large outlets

### Sales by Outlet Location
- Assessed geographic sales distribution across locations

### All Metrics by Outlet Type
- Combined KPIs (sales, ratings, item count, visibility) by outlet type

---

## Power BI Dashboard

The Power BI dashboard includes:
- KPI summary cards
- Sales breakdown by item type and fat content
- Outlet size and location-based analysis
- Interactive filters and slicers for exploration

---

## Repository Structure

```text
blinkit-sales-analysis/
│
├── README.md
│
├── sql/
│   └── query_doc.sql
│
├── python/
│   └── blinkit_analysis.ipynb
│
├── powerbi/
│   └── BlinkitDashboard.pbix
│
├── docs/
│   └── business_requirements.md
│
├── Dataset/
│
├── screenshots/
````

---

## Key Learnings

* Applied SQL for data cleaning and KPI computation
* Used Python for exploratory analysis and result validation
* Designed interactive Power BI dashboards for business insights
* Translated business requirements into analytical metrics
* Built an end-to-end analytics workflow

---

## Usage

This repository serves as:

* A portfolio project for data analytics roles
* A reference implementation for retail sales analysis
* A demonstration of SQL, Python, and Power BI integration

---

## Author

**Satyaprakash Singh Yadav**
Data Analytics | SQL | Python | Power BI

---

## Conclusion

This project demonstrates a complete data analytics workflow—from data preparation and KPI computation to visualization and insight generation—supporting informed decision-making in a retail analytics context.
