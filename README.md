# Blinkit Sales Performance Analysis  
**SQL | Python | Power BI**

## Overview

This project presents an **end-to-end sales performance analysis for Blinkit**, focusing on revenue trends, product performance, customer satisfaction, and outlet-level insights.

The analysis follows a structured analytics workflow:
- Business requirements definition
- Data preparation and validation
- KPI computation using SQL
- Exploratory analysis using Python
- Interactive visualization using Power BI

The project is designed to demonstrate a complete analytics lifecycle aligned with real-world business use cases.

---

## Business Objective

The primary objectives of this project are to:
- Evaluate overall sales performance
- Analyze product categories and fat content impact on sales
- Assess outlet-level and location-based performance
- Measure customer satisfaction using ratings
- Enable data-driven decision-making through KPIs and dashboards

Detailed business requirements are documented in:
```

docs/business_requirements.md

```

---

## Dataset Overview

The dataset contains structured retail sales data, including:
- Item and product attributes
- Fat content classification
- Outlet characteristics (type, size, location, establishment year)
- Sales values
- Customer ratings

The dataset files are available in the `Dataset/` directory.

---

## Analytics Workflow

### 1. SQL Analysis
SQL is used to perform:
- Data cleaning and standardization
- KPI computation
- Aggregation across multiple dimensions such as item type, outlet size, and location

The SQL analysis approach and logic are documented in:
```

docs/sql_analysis.md

```

---

### 2. Python Analysis
Python is used to:
- Perform exploratory data analysis (EDA)
- Validate KPI results derived from SQL
- Analyze grouped trends and distributions

The Python analysis methodology is documented in:
```

docs/python_analysis.md

```

---

### 3. Power BI Dashboard
Power BI is used to:
- Build an interactive dashboard
- Visualize KPIs and trends
- Enable filtering and drill-down analysis

The dashboard design and analytical logic are documented in:
```

docs/powerbi_dashboard.md

```

The Power BI file is available in:
```

powerbi/BlinkitDashboard.pbix

```

---

## Key Performance Indicators (KPIs)

The following KPIs are evaluated in this project:
- Total Sales
- Average Sales
- Number of Items Sold
- Average Customer Rating

These KPIs are analyzed across:
- Item type
- Fat content
- Outlet type
- Outlet size
- Outlet location
- Outlet establishment year

---

## Repository Structure

```

blinkit-sales-analysis/
│
├── README.md
│
├── Dataset/
│   ├── BlinkIT Grocery Data.csv
│   ├── BlinkIT Grocery Data.xlsx
│   └── BlinkIT_Data.csv
│
├── docs/
│   ├── business_requirements.md
│   ├── sql_analysis.md
│   ├── python_analysis.md
│   └── powerbi_dashboard.md
│
├── sql/
│   ├── query_doc.sql
│   └── Blinkit_SQL_Full_Analysis_With_Code_*.pdf
│
├── python/
│   └── Blinkit analysis.ipynb
│
├── powerbi/
│   └── BlinkitDashboard.pbix
│
├── screenshots/
│
└── README.md

```

---

## Key Insights

- Sales performance varies significantly across item categories and fat content
- Outlet size and location have a strong impact on total sales contribution
- Certain outlet types consistently outperform others
- Customer ratings provide additional context for sales performance evaluation

---

## Key Learnings

- Translated business requirements into analytical KPIs
- Applied SQL for structured data analysis and aggregation
- Used Python for exploratory analysis and validation
- Designed an interactive Power BI dashboard for business users
- Built a complete analytics workflow from raw data to insights

---

## Usage

This repository can be used as:
- A portfolio project for Data Analyst roles
- A reference for retail and e-commerce analytics
- A demonstration of SQL, Python, and Power BI integration

---

## Author

**Satyaprakash Singh Yadav**  
Data Analytics | SQL | Python | Power BI  

---

## Conclusion

This project demonstrates a complete and structured data analytics workflow, combining SQL-based analysis, Python validation, and Power BI visualization to generate actionable insights for retail sales performance.
