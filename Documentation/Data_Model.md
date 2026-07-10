# 🏗️ Data Model Documentation

## Overview

The dashboard is built using a **Star Schema** data model.

A Star Schema consists of one central Fact Table connected to multiple Dimension Tables.

This structure improves query performance, simplifies DAX calculations, and makes reporting easier.

---

# Data Model

The project contains the following tables:

## 1. Fact Table

The Fact Table stores all sales transactions.

It contains numerical business metrics such as:

- Total Sales
- Net Sales
- Profit
- Discount
- Discount Percentage
- Units Sold
- Price Per Unit

It also contains foreign keys linking to Dimension Tables.

---

## 2. Dimension Tables

### Dim Customers

Contains customer-related information.

Columns include:

- Customer ID
- Customer Name
- Email
- Phone Number
- City
- State
- Pincode

Purpose:

Provides customer-level analysis.

---

### Dim Products

Contains product information.

Columns include:

- Product ID
- Product Name
- Product Line
- Price Per Unit

Purpose:

Provides product-level analysis.

---

### Dim Promotion

Contains promotion details.

Columns include:

- Promotion Name
- Coupon Code
- Percentage
- Promotion Type

Purpose:

Used for discount and promotion analysis.

---

### Date Table 1

Acts as the primary Date Table.

Purpose:

Supports all standard date filtering and time-based analysis.

This table has an **Active Relationship** with the Fact Table.

---

### Date Table 2

Created specifically for comparing two different time periods.

Purpose:

Used with **USERELATIONSHIP()**.

This table has an **Inactive Relationship** with the Fact Table.

---

### Measures Table

Contains DAX Measures only.

Examples:

- Quantity Sold

Purpose:

Keeps the model clean and organizes business calculations separately from raw data.

---

# Relationships

The project uses:

## Relationship Type

One-to-Many (1:*)


Meaning:

One Product

↓

Many Sales Transactions

One Customer

↓

Many Sales Transactions

One Promotion

↓

Many Sales Transactions

---

## Cross Filter Direction

Single

Reason:

Single-direction filtering improves performance and avoids ambiguous relationships.

---

# Primary Keys

Dimension Tables contain Primary Keys.

Examples:

- Customer ID
- Product ID
- Promotion ID
- Date

These uniquely identify each record.

---

# Foreign Keys

The Fact Table stores Foreign Keys.

Examples:

- Customer ID
- Product ID
- Promotion ID
- Date

These connect the Fact Table with Dimension Tables.

---

# Active vs Inactive Relationships

## Active Relationship

Used for normal filtering.

Represented by a solid line in Power BI.

---

## Inactive Relationship

Used only when required.

Activated using:

```DAX
USERELATIONSHIP()
```

This enables comparison between two different date ranges.

---

# Why Star Schema?

Star Schema provides:

- Better performance
- Easier DAX calculations
- Simpler relationships
- Faster report generation
- Better scalability

---

# Model Design

The final model consists of:

- 1 Fact Table
- 3 Dimension Tables
- 2 Date Tables
- 1 Measures Table

This design follows Power BI best practices for analytical reporting.

---

# Concepts Demonstrated

- Star Schema
- Fact & Dimension Tables
- Primary Key
- Foreign Key
- One-to-Many Cardinality
- Single Cross Filter Direction
- Active Relationships
- Inactive Relationships
- USERELATIONSHIP()
- Measures Table