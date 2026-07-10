# 🎯 Power BI Project Interview Questions

This document contains interview questions that can be asked based on this project.

---

# Project Overview

## Q1. Explain your project.

**Answer:**

I built an interactive Sales Analytics Dashboard using Power BI. The project analyzes sales transactions and provides insights into sales, profit, product performance, promotions, customer behavior, and time-based trends. I used Power Query for data transformation, a Star Schema for data modeling, DAX for calculations, and interactive visuals for business reporting.

---

## Q2. Why did you choose Power BI?

**Answer:**

Power BI allows fast data transformation, efficient modeling, interactive dashboards, and powerful DAX calculations, making it ideal for business intelligence and analytics.

---

## Q3. What was the business problem?

**Answer:**

The objective was to transform raw sales data into an interactive dashboard that helps stakeholders analyze sales performance, identify top and bottom-performing products, compare time periods, and make data-driven decisions.

---

# Data Modeling

## Q4. What is a Star Schema?

**Answer:**

A Star Schema is a data modeling technique where one central Fact Table is connected to multiple Dimension Tables.

---

## Q5. Why did you use a Star Schema?

**Answer:**

- Better performance
- Simpler relationships
- Easier DAX calculations
- Faster report generation

---

## Q6. What is a Fact Table?

**Answer:**

A Fact Table stores transactional and numerical business data such as Sales, Profit, Discount, and Quantity Sold.

---

## Q7. What are Dimension Tables?

**Answer:**

Dimension Tables store descriptive information such as Customers, Products, Promotions, and Dates.

---

## Q8. Why did you create two Date Tables?

**Answer:**

One Date Table handles normal filtering. The second Date Table is used with USERELATIONSHIP() to compare two independent time periods.

---

## Q9. What is Cardinality?

**Answer:**

Cardinality defines how tables are related. This project uses One-to-Many relationships.

---

## Q10. Why Single Cross Filter Direction?

**Answer:**

Single-direction filtering improves model performance and avoids ambiguous relationships.

---

# Power Query

## Q11. Why did you use Power Query?

**Answer:**

Power Query was used for data cleaning, transformation, merging tables, changing data types, creating custom columns, and handling missing values before loading the data into the model.

---

## Q12. What transformations did you perform?

**Answer:**

- Changed data types
- Merge Queries
- Custom Columns
- Removed null values
- Calculated missing values
- Data Profiling

---

## Q13. Why use Power Query instead of DAX?

**Answer:**

Power Query performs data preparation before loading the model, reducing memory usage and improving report performance. DAX is better suited for dynamic calculations after the data has been loaded.

---

# DAX

## Q14. What DAX measures did you create?

**Answer:**

- Total Sales
- Net Sales
- Profit
- Quantity Sold

---

## Q15. What is CALCULATE()?

**Answer:**

CALCULATE() modifies the filter context before evaluating an expression.

---

## Q16. What is USERELATIONSHIP()?

**Answer:**

USERELATIONSHIP() temporarily activates an inactive relationship for a specific calculation.

---

## Q17. Why did you use USERELATIONSHIP()?

**Answer:**

To compare Sales, Profit, and Quantity Sold between two different user-selected time periods.

---

## Q18. Why did you create a Measures Table?

**Answer:**

To organize all DAX measures separately from raw data tables, improving readability and maintainability.

---

# Dashboard

## Q19. Why did you use KPI Cards?

**Answer:**

To display important business metrics such as Sales, Profit, Quantity Sold, and Number of Orders.

---

## Q20. Why did you use Bar Charts?

**Answer:**

To compare product performance across different categories.

---

## Q21. Why did you use a Scatter Plot?

**Answer:**

To analyze the relationship between Net Sales and Profit.

---

## Q22. Why did you use a Map Visual?

**Answer:**

To analyze sales distribution across different cities.

---

## Q23. Why did you use a Table Visual?

**Answer:**

To provide detailed transaction-level information.

---

# Interactive Features

## Q24. What are Dynamic Slicers?

**Answer:**

Dynamic slicers display only values that have corresponding data after current filters are applied.

---

## Q25. Why did you use a Net Sales measure in slicer filters?

**Answer:**

To hide blank values and display only relevant options to users.

---

## Q26. What is Drill Through?

**Answer:**

Drill Through allows users to navigate from summary visuals to detailed information about selected data.

---

## Q27. What are Edit Interactions?

**Answer:**

Edit Interactions controls how slicers and visuals affect each other, enabling independent filtering.

---

# Project

## Q28. What challenges did you face?

**Answer:**

Understanding data modeling, inactive relationships, DAX filter context, and implementing dynamic comparisons between two time periods.

---

## Q29. If you improve this project, what would you add?

**Answer:**

- Forecasting
- KPI Trend Indicators
- Row-Level Security
- Better Dashboard UI
- Power BI Service Deployment

---

## Q30. What did you learn from this project?

**Answer:**

This project improved my understanding of Power Query, data cleaning, Star Schema, DAX, relationships, dashboard design, and business analytics. It also strengthened my ability to build interactive dashboards that answer real business questions.