# SQL_DEVELOPER_INTERNSHIP_TASK4

# Task 4: Aggregate Functions and Grouping (SQL Developer Internship)

## 📌 Objective
Use aggregate functions and `GROUP BY` to summarize and analyze data from database tables.

## 🛠 Tools Used
- DB Browser for SQLite / MySQL Workbench  
- SQL

## 📂 Files in This Repository
- **task4.sql** → Contains SQL queries for:
  - `SUM`
  - `COUNT`
  - `AVG`
  - `GROUP BY`
  - `HAVING`
- **README.md** → Documentation and explanation

---

## 📊 Sample Data

### Employees Table
| emp_id | name   | department   | salary   |
|--------|--------|-------------|----------|
| 1      | Asha   | Engineering | 95000    |
| 2      | Rahul  | Engineering | 105000   |
| 3      | Meera  | HR          | 65000    |
| ...    | ...    | ...         | ...      |

### Sales Table
| sale_id | order_date | product    | category     | region | customer_id | quantity | price  |
|---------|------------|------------|--------------|--------|-------------|----------|--------|
| 1       | 2024-01-05 | Laptop     | Electronics  | North  | 101         | 2        | 50000  |
| 2       | 2024-01-06 | Mouse


## 📜 Queries Included

### 1️⃣ Basic Aggregates
- **Total Revenue**
sql
SELECT SUM(quantity * price) AS total_revenue
FROM sales;


💡 Key Learnings

GROUP BY is used to group rows based on one or more columns.
HAVING filters groups after aggregation.
COUNT(*) counts all rows; COUNT(column) ignores NULLs.
ROUND() helps format numeric output.
Multiple columns can be used in GROUP BY for more specific groupings.
