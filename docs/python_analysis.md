# Blinkit Sales Analysis – Python Workflow

## Overview

This document describes the **Python-based analysis** performed for the Blinkit Sales Performance project.  
Python is used to validate data quality, perform exploratory analysis, and cross-check key performance indicators computed using SQL and visualized in Power BI.

The Python layer acts as a **verification and exploratory analytics layer** within the overall data analytics workflow.

---

## Environment and Libraries

The analysis is performed using standard Python data analysis libraries:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
````

* **Pandas:** Data manipulation and aggregation
* **NumPy:** Numerical operations
* **Matplotlib / Seaborn:** Exploratory visualization

---

## Data Loading

The dataset is loaded into a Pandas DataFrame for structured analysis.

```python
df = pd.read_csv("blinkit_data.csv")
df.head()
```

This step confirms successful ingestion and provides an initial view of the dataset.

---

## Data Inspection and Validation

Basic inspection is performed to understand schema, data types, and missing values.

```python
df.info()
df.isnull().sum()
```

These checks ensure:

* Correct data types for numerical and categorical fields
* Awareness of missing or incomplete records
* Readiness for aggregation and KPI computation

---

## Data Cleaning and Standardization

Categorical values are standardized to ensure consistency with SQL-based analysis.

```python
df['Item_Fat_Content'] = df['Item_Fat_Content'].replace({
    'LF': 'Low Fat',
    'low fat': 'Low Fat',
    'reg': 'Regular'
})
```

This step prevents incorrect grouping and aggregation during analysis.

---

## KPI Computation

Key business KPIs are computed using Pandas aggregation functions.

```python
total_sales = df['Total_Sales'].sum()
avg_sales = df['Total_Sales'].mean()
number_of_items = df.shape[0]
avg_rating = df['Rating'].mean()
```

These metrics are cross-validated with SQL-derived KPIs.

---

## Grouped Analysis

Aggregations are performed to analyze performance across different dimensions.

```python
sales_by_fat_content = df.groupby('Item_Fat_Content')['Total_Sales'].sum()
sales_by_outlet_type = df.groupby('Outlet_Type')['Total_Sales'].sum()
```

This enables comparison of sales patterns across product and outlet attributes.

---

## Exploratory Visualization

Basic visualizations are created to support exploratory analysis and trend validation.

```python
sales_by_fat_content.plot(kind='bar', title='Sales by Fat Content')
plt.show()
```

These visuals help confirm trends later presented in Power BI dashboards.

---

## Role of Python in This Project

Python is used to:

* Validate raw and cleaned data
* Perform exploratory analysis
* Cross-check SQL-based KPI calculations
* Support analytical reasoning before visualization

---

## Conclusion

The Python analysis layer strengthens the overall analytics pipeline by ensuring data consistency, validating KPIs, and enabling exploratory insights prior to dashboard development.

