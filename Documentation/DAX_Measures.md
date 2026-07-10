# 📐 DAX Measures Documentation

## Overview

This document explains the DAX measures and functions used in the Sales Analytics Dashboard.

DAX (Data Analysis Expressions) was used to create business calculations and enable dynamic report interactions.

---

# Total Sales

```DAX
Total Sales = SUM('Fact Table'[Total Sales])
```

### Purpose

Calculates the total sales generated across all transactions.

### Used In

- KPI Cards
- Sales Comparison
- Product Analysis

---

# Net Sales

```DAX
Net Sales = SUM('Fact Table'[Net Sales])
```

### Purpose

Calculates the total Net Sales after discounts.

### Used In

- Sales Comparison
- Dynamic Slicers
- Scatter Plot

---

# Profit

```DAX
Profit = SUM('Fact Table'[Profit])
```

### Purpose

Calculates the total profit earned.

### Used In

- KPI Cards
- Product Analysis
- Scatter Plot

---

# Quantity Sold

```DAX
Quantity Sold = SUM('Fact Table'[Units Sold])
```

### Purpose

Calculates the total number of units sold.

### Used In

- KPI Cards
- Product Analysis
- Time Comparison

---

# USERELATIONSHIP()

Example:

```DAX
Sales Comparison =
CALCULATE(
    [Net Sales],
    USERELATIONSHIP(
        'Date Table 2'[Date],
        'Fact Table'[Date (dd/mm/yyyy)]
    )
)
```

### Purpose

Temporarily activates the inactive relationship between **Date Table 2** and the **Fact Table**.

### Why It Was Used

The dashboard compares Sales, Profit, and Quantity Sold between two user-selected time periods.

Since only one relationship can be active at a time, USERELATIONSHIP() allows the second Date Table to participate in calculations.

---

# CALCULATE()

Purpose:

Changes the filter context before evaluating an expression.

Example:

```DAX
CALCULATE(
    [Net Sales],
    USERELATIONSHIP(...)
)
```

Used to evaluate measures under a different relationship.

---

# SUM()

Purpose:

Adds all values in a numeric column.

Example:

```DAX
SUM('Fact Table'[Profit])
```

Used for creating KPI measures.

---

# Dynamic Slicer Measure

A Net Sales measure was added to slicers as a **Visual Level Filter**.

Filter Condition:

```
Show items when value is NOT BLANK
```

Purpose:

Only display slicer values that contain matching records after filters are applied.

This creates dynamic slicers and prevents users from selecting options that would return empty visuals.

---

# DAX Concepts Demonstrated

- Measures
- SUM()
- CALCULATE()
- USERELATIONSHIP()
- Filter Context
- Active Relationships
- Inactive Relationships
- Dynamic Filtering

---

# Interview Questions

### Why use Measures instead of Calculated Columns?

Measures are calculated dynamically based on the current filter context and consume less storage.

---

### Why use CALCULATE()?

To modify the filter context before evaluating an expression.

---

### Why use USERELATIONSHIP()?

To temporarily activate an inactive relationship between the second Date Table and the Fact Table.

---

### Why use a separate Measures Table?

To organize DAX measures separately from raw data tables, making the model cleaner and easier to maintain.