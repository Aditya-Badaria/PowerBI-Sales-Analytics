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

## ⭐ Repository Highlights

- End-to-end Power BI project
- Power Query for ETL
- Star Schema data model
- Interactive DAX measures
- Dynamic time-period comparison
- Comprehensive project documentation
- Git version control

---

## 🛠️ Tech Stack

- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel
- Git & GitHub

---

## 📂 Dataset

## 📂 Dataset

The project uses a retail sales dataset containing transactional information related to customers, products, promotions, and sales.

The dataset was provided as part of the Power BI module in **Krish Naik's Complete Data Analyst Bootcamp** and is used here for educational and portfolio purposes.

---

## 📚 Learning Source

This project was completed as part of my learning journey through **Krish Naik's _Complete Data Analyst Bootcamp: Basics to Advanced_** on Udemy.

The dataset and guided workflow were provided in the course. I independently implemented the complete dashboard, documented the project, and focused on understanding concepts such as Power Query, Star Schema, DAX, relationships, and interactive dashboard design.

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

- Annual Sales Trend Analysis
- Custom Time Period Comparison

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

## 📈 Key Business Insights

Based on the dashboard analysis, the following business insights were identified:

### Product Performance

- Apple iPhone 14 emerged as the highest revenue-generating product with approximately **21.4M** in sales and also ranked first in overall profit.
- Apple MacBook Air and Sony Bravia 55" TV were also among the top-performing products, indicating strong demand for premium electronics.
- Products such as **Tupperware Lunch Box**, **L'Oreal Shampoo**, and **Colgate Toothpaste** generated the lowest sales and profit, suggesting opportunities to review pricing, promotions, or inventory strategy.

---

### Sales & Profit Analysis

- The scatter plot shows a strong positive relationship between **Net Sales** and **Profit**, indicating that higher sales generally resulted in higher profitability across transactions.
- No major outliers were observed, suggesting relatively consistent profit margins throughout the dataset.

---

### Promotion Analysis

- **Weekend Flash Sale** offered the highest average discount, followed by **Clearance Sale**.
- **Festive Diwali** promotions showed little or no discount activity in the available dataset, which may indicate limited campaign usage or missing promotional transactions.

---

### Time Trend Analysis

- Annual sales remained relatively stable between **2020** and **2023**, fluctuating between **29M** and **32M**.
- The 2024 value appears significantly lower because the available dataset may contain only partial-year records rather than a complete year's sales.

---

### Geographic Analysis

- Sales transactions were distributed across multiple major Indian cities, indicating a geographically diversified customer base.
- Cities with larger map markers contributed higher sales volumes and may represent key regional markets for future business growth.

---

### Comparative Analysis

- The dashboard enables users to compare **Sales**, **Profit**, and **Quantity Sold** between any two custom date ranges using independent date slicers.
- This functionality helps identify seasonal trends and evaluate business performance across different periods.

---

### Operational Insights

- The interactive transaction table allows users to drill down into individual sales records using filters for Date, Customer, Product, and Promotion.
- Dynamic slicers ensure that only relevant filter values are displayed, improving user experience and preventing empty selections.

---

## 💼 Business Recommendations

- Increase inventory availability for high-performing products such as Apple iPhone 14 and Apple MacBook Air to avoid stock shortages.
- Re-evaluate pricing and promotional strategies for consistently low-performing products.
- Analyze the effectiveness of high-discount campaigns to ensure that increased discounts are translating into higher profitability.
- Focus marketing efforts on cities contributing the highest sales while exploring opportunities in lower-performing regions.
- Use the time-period comparison dashboard to monitor seasonal demand and optimize future promotional campaigns.

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

## 🚀 Future Improvements

- Deploy the report using Power BI Service.
- Implement Row-Level Security (RLS) for role-based access.
- Add advanced KPI indicators and dynamic tooltips.
- Incorporate forecasting and time-series analytics.
- Enhance the dashboard UI for executive reporting.

---

# 👨‍💻 Author

**Aditya Badaria**

B.Tech, Computer Science Engineering  
Punjab Engineering College (PEC), Chandigarh

📧 Feel free to connect for feedback, collaboration, or discussions on Data Analytics and Business Intelligence.