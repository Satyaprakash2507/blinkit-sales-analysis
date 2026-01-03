# SQL Analysis Documentation – Blinkit Sales Project

## Overview

This document explains how **SQL** was used in the Blinkit Sales Analysis project to perform data cleaning, aggregation, and KPI computation.  
SQL served as the primary layer for structured data analysis and metric generation before validation and visualization.

The focus of this document is on **analytical intent and business logic**, not query syntax.

---

## Role of SQL in This Project

SQL was used to:
- Explore the dataset structure
- Clean and standardize categorical values
- Compute core business KPIs
- Perform dimensional analysis across products and outlets
- Prepare aggregated datasets for visualization and validation

---

## Data Understanding and Exploration

Initial data exploration was performed to:
- Review available columns and data types
- Understand sales, rating, and outlet attributes
- Identify inconsistencies in categorical fields
- Validate record counts and completeness

This step ensured that downstream analysis was based on reliable data.

---

## Data Cleaning and Standardization

### Fat Content Normalization

The `Item_Fat_Content` field contained multiple representations for the same category.  
These values were standardized to ensure consistent grouping and aggregation.

**Business Impact:**
- Prevents incorrect KPI calculations
- Ensures accurate comparison across product categories
- Improves reliability of visual insights

---

## Key Performance Indicator (KPI) Computation

SQL was used to compute the following KPIs:

### Total Sales
- Measures overall revenue generated
- Used as the primary performance indicator

### Average Sales
- Indicates average transaction value
- Helps assess pricing and sales consistency

### Number of Items Sold
- Represents total item-level demand
- Useful for understanding product movement

### Average Rating
- Serves as a proxy for customer satisfaction
- Used to correlate product quality with sales performance

---

## Dimensional Sales Analysis

SQL aggregations were applied to analyze sales across multiple dimensions:

### Sales by Fat Content
- Compared revenue contribution of low-fat and regular products
- Evaluated how product composition affects total sales

### Sales by Item Type
- Identified top-performing product categories
- Supported category-level optimization decisions

### Sales by Outlet Location
- Assessed geographic distribution of sales
- Highlighted high-performing outlet regions

### Sales by Outlet Size
- Analyzed contribution of small, medium, and large outlets
- Supported capacity and expansion planning insights

### Sales by Outlet Establishment Year
- Evaluated the relationship between outlet age and sales
- Identified maturity trends across outlets

---

## Advanced Aggregation Logic

SQL techniques were used to:
- Calculate percentage contribution of sales
- Compare metrics across outlet dimensions
- Create pivot-style summaries for clearer comparison

These aggregations enabled multi-dimensional analysis without duplicating logic in visualization tools.

---

## Validation and Consistency Checks

SQL outputs were cross-validated by:
- Comparing aggregated values with Python analysis
- Ensuring KPI consistency with Power BI measures
- Reviewing grouped results for logical correctness

This ensured analytical integrity across tools.

---

## Usage in the Overall Project

In this project, SQL acted as:
- The foundation for KPI computation
- The primary source for structured aggregations
- A validation layer for analytics and visualization

---

## Conclusion

SQL played a critical role in transforming raw retail data into structured, business-ready metrics.  
By combining data cleaning, aggregation, and dimensional analysis, SQL enabled accurate and scalable sales performance evaluation for Blinkit.
