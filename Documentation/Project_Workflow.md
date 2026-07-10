# 📊 Power BI Sales Analytics Dashboard - Project Workflow

## Objective

The objective of this project is to analyze retail sales data and build an interactive Power BI dashboard that provides meaningful business insights related to sales, profit, products, customers, promotions, and time-based performance.

---

# Project Workflow

## Step 1: Data Collection

- Imported the dataset from Microsoft Excel.
- The dataset contained multiple tables:
  - Fact Table
  - Dim Customers
  - Dim Products
  - Dim Promotions

---

## Step 2: Data Cleaning & Transformation

Performed data preprocessing using **Power Query**.

Tasks performed:

- Checked data quality using Data Profiling.
- Corrected incorrect data types.
- Replaced missing values.
- Merged tables using Merge Queries.
- Created Custom Columns for missing business metrics.
- Calculated Discount, Net Sales and other required fields.
- Removed unnecessary null values.

---

## Step 3: Data Modeling

Designed the data model using **Star Schema**.

Created relationships between:

- Fact Table
- Product Dimension
- Customer Dimension
- Promotion Dimension
- Date Table

Relationship Type:

- One-to-Many

Cross Filter Direction:

- Single

Also created a second Date Table for time-period comparison using USERELATIONSHIP().

---

## Step 4: DAX Measures

Created DAX measures to calculate business metrics.

Examples:

- Total Sales
- Quantity Sold

Also used:

- CALCULATE()
- USERELATIONSHIP()

to compare two different time periods.

---

## Step 5: Dashboard Development

Created multiple interactive report pages including:

- Dashboard Overview
- Top & Bottom Product Analysis
- Time Period Comparison
- Transaction Details

Visuals used:

- KPI Cards
- Bar Charts
- Line Charts
- Scatter Plot
- Table Visual
- Map Visual
- Slicers

---

## Step 6: Interactive Features

Implemented several interactive Power BI features.

- Dynamic Slicers
- Drill Through
- Edit Interactions
- USERELATIONSHIP()
- Dynamic Filtering

These features improve dashboard usability and allow users to explore data efficiently.

---

## Step 7: Documentation & Version Control

The completed project was:

- Organized into a structured folder hierarchy.
- Uploaded to GitHub.
- Documented using Markdown.
- Version controlled using Git.

---

# Workflow Summary

Excel Dataset

↓

Power Query

↓

Data Cleaning

↓

Star Schema

↓

Relationships

↓

DAX Measures

↓

Interactive Dashboard

↓

GitHub Documentation

---

## Skills Demonstrated

- Data Cleaning
- Data Transformation
- Data Modeling
- DAX
- Power BI Visualization
- Dashboard Design
- Business Analysis
- Git & GitHub