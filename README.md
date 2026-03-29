# 🏦 Banking Management System - SQL Queries

This project features a banking database schema and a collection of SQL problem-solving queries. 
---

## 📂 Project Overview

This repository contains:
1.  **`sample-db.sql`**: A complete database dump including table structures (schema) and sample data for customers, accounts, employees, branches, and transactions.
2.  **`sql-qa.txt`**: A set of common banking-related problem statements solved using optimized MySQL queries.

---

## 🏗️ Database Schema

The database consists of the following interconnected tables:

### 👥 Customer Management
- **`customer`**: Central repository for all customer IDs and addresses.
- **`individual`**: Detailed information for personal account holders.
- **`business`**: Information for corporate clients.
- **`officer`**: Details of officers associated with business accounts.

### 💰 Accounts & Transactions
- **`account`**: Vital statistics like available balance, status (Active/Closed), and product codes.
- **`acc_transaction`**: Historical record of all financial movements.
- **`product` & `product_type`**: Definition of bank offerings (Savings, Checking, Loans, etc.).

### 🏢 Internal Operations
- **`branch`**: Physical bank locations and headquarters.
- **`employee`**: Staff details including hierarchy, salaries, and department affiliations.
- **`department`**: Internal organizational structure (IT, Loans, Operations, etc.).

---

## 📊 SQL Practice Highlights

The project includes solutions for real-world scenarios, such as:
- **Salary Analysis**: Finding nth highest salaries using subqueries.
- **Data Aggregation**: Grouping accounts by branches and filtering based on average balances.
- **Pagination**: Implementing efficient data fetching strategies for large datasets.
- **Statistics**: Counting distinct operational branches across the system.

### Example Query: Finding 2nd Highest Salary
```sql
SELECT MAX(salary) AS Second_Highest_Salary
FROM employee
WHERE salary < (SELECT MAX(salary) FROM employee);
```


## 🛠️ Built With
- **MySQL**: Relational Database Management System.
- **SQL**: Structured Query Language.

---

*Happy Querying!* 🚀
