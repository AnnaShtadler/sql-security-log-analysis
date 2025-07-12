# 🛡️ SQL Log Analysis: Investigating Suspicious Login Attempts

This project simulates the role of a security analyst investigating suspicious login activity within a large organization. Using SQL queries, I filtered and analyzed data from employee and login tables to detect anomalies, improve system security, and ensure up-to-date machine configurations.

---

## 📌 Project Objectives

- Identify failed login attempts outside of working hours
- Filter login attempts by date and country
- Exclude specific departments from system updates
- Select employees from specific departments and office locations

---

## 🧠 SQL Concepts Used

- Logical operators: `AND`, `OR`, `NOT`
- Comparison operators: `=`, `>`, `LIKE`
- Wildcard pattern matching: `'MEX%'`, `'East-%'`
- Filtering data based on multiple conditions

---

## 🗂️ Files

| File             | Description                                    |
| ---------------- | ---------------------------------------------- |
| `Portfolio2.pdf` | Full report with SQL queries and explanations  |
| `README.md`      | This file – project overview and documentation |


---

## 📄 Sample SQL Query

```sql
SELECT * 
FROM log_in_attempts
WHERE login_time > '18:00' AND success = FALSE;
