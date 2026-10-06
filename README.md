<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,50:1E3A8A,100:06B6D4&height=220&section=header&text=SQL%20Data%20Analysis&fontSize=45&fontColor=FFFFFF&animation=fadeIn&fontAlignY=35" width="100%">
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=25&duration=2500&pause=800&color=06B6D4&center=true&vCenter=true&width=800&lines=E-Commerce+SQL+Data+Analysis;Database+Design+%26+Querying;Revenue+%26+Customer+Analytics;SQL+Joins+%7C+Subqueries+%7C+Views;Query+Optimization+%26+Indexing" alt="Typing Animation">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/SQL-Data%20Analysis-06B6D4?style=for-the-badge&logo=sqlite&logoColor=white">
  <img src="https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white">
  <img src="https://img.shields.io/badge/E--Commerce-Analytics-8B5CF6?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Completed-22C55E?style=for-the-badge">
</p>

<p align="center">
  <b>SQL for Data Analysis | E-Commerce Database | SQLite</b>
</p>

---

# 📌 Project Overview

This project demonstrates practical SQL skills for analyzing structured e-commerce data.

An e-commerce database was designed using SQLite with separate tables for customers, products, orders, and order items.

SQL queries were developed to extract, transform, aggregate, and analyze the data.

The project covers fundamental as well as practical SQL concepts including:

- Data retrieval
- Filtering
- Sorting
- Grouping
- Aggregate functions
- JOIN operations
- Subqueries
- Views
- NULL handling
- Indexing
- Query optimization
- Business-oriented revenue analysis

---

# 🎯 Project Objective

The main objective is to use SQL queries to extract and analyze meaningful information from an e-commerce database.

The project focuses on transforming raw structured data into useful business insights.

### Key Objectives

- Create a structured e-commerce database
- Insert and manage sample data
- Retrieve records using SQL
- Filter records using `WHERE`
- Sort records using `ORDER BY`
- Group data using `GROUP BY`
- Perform calculations using aggregate functions
- Combine tables using JOINs
- Use subqueries for advanced analysis
- Create reusable SQL views
- Handle NULL values
- Improve query performance using indexes
- Analyze SQL execution plans
- Calculate business metrics such as revenue and ARPU

---

# 🗂️ Database Architecture

The database consists of four major tables.

```text
                         ┌─────────────────────┐
                         │      CUSTOMERS      │
                         ├─────────────────────┤
                         │ customer_id         │
                         │ customer_name       │
                         │ email               │
                         │ city                │
                         │ country             │
                         └──────────┬──────────┘
                                    │
                                    │ customer_id
                                    ▼
                         ┌─────────────────────┐
                         │       ORDERS        │
                         ├─────────────────────┤
                         │ order_id            │
                         │ customer_id         │
                         │ order_date          │
                         │ total_amount        │
                         └──────────┬──────────┘
                                    │
                                    │ order_id
                                    ▼
                         ┌─────────────────────┐
                         │    ORDER_ITEMS      │
                         ├─────────────────────┤
                         │ order_item_id       │
                         │ order_id            │
                         │ product_id          │
                         │ quantity            │
                         │ unit_price          │
                         └──────────┬──────────┘
                                    │
                                    │ product_id
                                    ▼
                         ┌─────────────────────┐
                         │      PRODUCTS       │
                         ├─────────────────────┤
                         │ product_id          │
                         │ product_name        │
                         │ category            │
                         │ price               │
                         └─────────────────────┘
