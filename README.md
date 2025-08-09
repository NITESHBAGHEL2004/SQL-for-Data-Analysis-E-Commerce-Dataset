# 🛍️ Task 4: SQL for Data Analysis – E-Commerce Dataset

## 📌 Objective
The goal of this task is to **extract and analyze data** from an e-commerce database using SQL.  
We demonstrate the use of **SELECT, WHERE, ORDER BY, JOINS, Subqueries, Aggregate Functions, Views, and Index Optimization**.

---

## 📂 Files in this Repository
- **`ecommerce.db`** – Sample SQLite database with:
  - Customers table
  - Products table
  - Orders table
  - Order Items table
- **`task4_queries.sql`** – All SQL queries for Task 4.
- **`README.md`** – This documentation.

---

## 🗄️ Database Schema

**customers**
| Column       | Type    |
|--------------|---------|
| customer_id  | INTEGER |
| name         | TEXT    |
| country      | TEXT    |

**products**
| Column       | Type    |
|--------------|---------|
| product_id   | INTEGER |
| product_name | TEXT    |
| category     | TEXT    |
| price        | REAL    |

**orders**
| Column       | Type    |
|--------------|---------|
| order_id     | INTEGER |
| customer_id  | INTEGER |
| order_date   | TEXT    |

**order_items**
| Column       | Type    |
|--------------|---------|
| item_id      | INTEGER |
| order_id     | INTEGER |
| product_id   | INTEGER |
| quantity     | INTEGER |

---

## 🛠️ Tools Used
- **SQLite** (You can also adapt queries for MySQL or PostgreSQL)
- Any SQL viewer (DB Browser for SQLite recommended)

---

## 📜 SQL Features Demonstrated
1. **Basic Queries** – `SELECT`, `WHERE`, `ORDER BY`
2. **Joins** – `INNER JOIN`
3. **Subqueries** – Filtering based on aggregated results
4. **Aggregate Functions** – `SUM()`, `AVG()`
5. **Views** – Creating reusable query results
6. **Indexes** – (optional) for query optimization

---

## ▶️ How to Run
1. Download `ecommerce.db` and `task4_queries.sql`
2. Open `ecommerce.db` in your SQL tool
3. Copy & paste queries from `task4_queries.sql` or run directly:
   ```bash
   sqlite3 ecommerce.db < task4_queries.sql
