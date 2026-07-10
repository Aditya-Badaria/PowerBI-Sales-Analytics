![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green)
![DAX](https://img.shields.io/badge/DAX-Data%20Analysis-blue)
![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?logo=github)

# 📊 Power BI Sales Analytics Dashboard

An interactive Sales Analytics Dashboard built using **Power BI**, **Power Query**, and **DAX** to analyze sales performance, product profitability, promotions, customer behavior, and time-based trends.

---

## 📌 Project Overview

This project analyzes a retail sales dataset and transforms raw transactional data into an interactive dashboard that helps businesses monitor KPIs and make data-driven decisions.

The dashboard allows users to:

- Analyze Sales, Profit, and Quantity Sold
- Compare Top & Bottom Performing Products
- Compare two different time periods
- Analyze promotional discounts
- View sales geographically
- Drill through transaction-level details
- Filter the dashboard dynamically using slicers

---

## 🛠️ Tech Stack

- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel
- Git & GitHub

---

## 📂 Dataset

The project uses a retail sales dataset containing:

- Customer Information
- Product Information
- Promotion Details
- Sales Transactions

---

## 🏗️ Data Model

The dashboard follows a **Star Schema** consisting of:

- Fact Table
- Customer Dimension
- Product Dimension
- Promotion Dimension
- Two Date Tables
- Dedicated Measures Table

Relationships were created using **Primary Keys** and **Foreign Keys** with One-to-Many cardinality.

---

## 📊 Dashboard Features

### Executive Dashboard

- Total Sales
- Total Profit
- Total Quantity Sold
- Number of Orders

### Product Analysis

- Top 5 Products by Sales
- Bottom 5 Products by Sales
- Top 5 Products by Profit
- Bottom 5 Products by Profit
- Top & Bottom Products by Quantity

### Time Analysis

- Sales Trend by Year
- Compare Sales between any two selected periods

### Promotion Analysis

- Average Discount by Promotion Category

### Geographic Analysis

- Sales by City using Map Visual

### Interactive Features

- Dynamic Slicers
- Drill Through
- USERELATIONSHIP()
- Edit Interactions
- Dynamic Filtering

---

## 📷 Dashboard Preview
### 1. Dashboard Overview

![Dashboard Overview](Dashboard%20Screenshots/01_Dashboard_Overview.png)

---

### 2. Top & Bottom Product Analysis

This dashboard identifies the best and worst performing products based on **Sales, Profit, and Quantity Sold**.

![Top Bottom Products](Dashboard%20Screenshots/02_Top_Bottom_Products.png)

---

### 3. Time Period Comparison

Compare **Sales, Profit, and Quantity Sold** between any two user-selected time periods using independent date slicers implemented with **USERELATIONSHIP()** and **Edit Interactions**.

![Time Period Comparison](Dashboard%20Screenshots/03_Time_Period_Comparison.png)

---

### 4. Transaction Details

A detailed transaction table with dynamic filtering using Date, Customer, Product, and Promotion slicers.

![Detailed Sales Table](Dashboard%20Screenshots/04_Detailed_Sales_Table.png)

---

### 5. Data Model

The project follows a **Star Schema** consisting of one Fact Table, multiple Dimension Tables, dedicated Measures Table, and two Date Tables (one active and one inactive relationship).

![Data Model](Dashboard%20Screenshots/05_Data_Model.png)

---

# 💡 Key Features

- ✔ Data Cleaning & Transformation using Power Query
- ✔ Star Schema Data Modeling
- ✔ One-to-Many Relationships
- ✔ DAX Measures
- ✔ USERELATIONSHIP() for Time Comparison
- ✔ Interactive Slicers
- ✔ Drill Through Navigation
- ✔ Dynamic Visual Filtering
- ✔ Geographic Analysis using Map Visual
- ✔ KPI Cards
- ✔ Top & Bottom Product Analysis

---

# 🧠 Concepts Implemented

### Power Query

- Merge Queries
- Custom Columns
- Data Cleaning
- Data Type Transformation
- Handling Missing Values

### Data Modeling

- Star Schema
- Primary Keys & Foreign Keys
- One-to-Many Cardinality
- Active & Inactive Relationships

### DAX

- CALCULATE()
- USERELATIONSHIP()
- SUM()
- Dynamic Measures

### Visualizations

- Bar Charts
- Line Charts
- Scatter Plot
- Map Visual
- Card Visual
- Table Visual
- Slicers

---

# 📁 Project Structure

```text
PowerBI-Sales-Analytics
│
├── Dashboard Screenshots/
├── Dataset/
├── Documentation/
├── PowerBI/
│   └── Sales Analytics Dashboard.pbix
├── README.md
└── .gitignore
```

---

# 🚀 Future Improvements

- Publish the dashboard to Power BI Service.
- Add Row-Level Security (RLS).
- Implement advanced KPI indicators.
- Add forecasting for future sales.
- Improve dashboard theme and UI.

---

# 👨‍💻 Author

**Aditya Badaria**

B.Tech Computer Science Engineering  
Punjab Engineering College (PEC), Chandigarh

If you found this project helpful, feel free to ⭐ this repository.