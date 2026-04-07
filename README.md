# FreshMart Stock Health Report

A SQL-based inventory analysis system for FreshMart supermarket chain.  
This project identifies products nearing expiration and those with no recent sales activity.

---

## Project Overview

FreshMart was facing losses due to overstocking products that don't sell and running out of products that do. This SQL script provides three targeted reports to help the Inventory Manager make data-driven decisions.

---

## Database Schema

Three tables are used in this project:

**Categories** — stores product category names  
**Products** — stores product details including stock, expiry, and pricing  
**SalesTransactions** — records every sale made against a product

---

## Reports

### Report 1 — Expiring Soon
Finds all products expiring within the next 7 days that still have more than 50 units in stock.  
This helps the team take quick action — discounts, promotions, or returns — before the stock becomes a total loss.

### Report 2 — Dead Stock
Identifies products that have had zero sales in the last 60 days.  
These products are occupying shelf space and warehouse capacity without generating any revenue.

### Report 3 — Revenue by Category
Shows which product category generated the most revenue in the last month.  
This helps management decide where to invest more shelf space and budget.

---

## How to Run

1. Open MySQL Workbench and connect to your local server
2. Open a new query tab
3. Run the full script in this order:
   - Create the database and tables
   - Insert the sample data
   - Run each report query one at a time

```sql
CREATE DATABASE FreshMart;
USE FreshMart;
```

Then paste and run the rest of the script.

---

## Files in This Repository

| File | Description |
|---|---|
| `freshmart_stock_report.sql` | Complete SQL script with schema, data, and all 3 reports |
| `Query_Explanation.docx` | Detailed explanation of each query with logic and reasoning |
| `README.md` | This file |

---

## Tech Stack

- MySQL 8.x
- MySQL Workbench

---

## Author

Developed as part of an internship assignment to demonstrate SQL schema design and query writing skills.
