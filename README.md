# 📚 Book Store Management System | PostgreSQL SQL Project

## 📖 Project Overview

This project demonstrates how PostgreSQL can be used to manage and analyze data for a bookstore. It covers the complete workflow of designing a relational database, importing CSV datasets, and writing SQL queries to solve real-world business problems.

The project focuses on customer purchases, inventory management, sales analysis, and revenue insights while practicing essential SQL concepts used in data analytics.

---

## 🗂️ Database Structure

The database consists of three related tables.

### 📘 Books

Stores information about every book available in the bookstore.

**Columns**

- Book_ID
- Title
- Author
- Genre
- Published_Year
- Price
- Stock

### 👤 Customers

Stores customer details.

**Columns**

- Customer_ID
- Name
- Email
- Phone
- City
- Country

### 🛒 Orders

Stores purchase records for customers.

**Columns**

- Order_ID
- Customer_ID
- Book_ID
- Order_Date
- Quantity
- Total_Amount

---

## 🔗 Table Relationships

| Parent Table | Child Table | Relationship |
|--------------|------------|--------------|
| Customers | Orders | One Customer can place many Orders (1:N) |
| Books | Orders | One Book can appear in many Orders (1:N) |

---

## 📂 Dataset Information

The project uses three CSV files:

- **Books.csv** – Book details including title, author, genre, price, and stock.
- **Customers.csv** – Customer information.
- **Orders.csv** – Customer purchase history.

All datasets were imported into PostgreSQL using the `COPY` command.

---

## 🛠 SQL Concepts Practiced

Throughout this project, the following SQL concepts were used:

- Database Creation
- Table Creation
- Primary Keys
- Foreign Keys
- Data Import using `COPY`
- Data Filtering (`WHERE`)
- Sorting (`ORDER BY`)
- Aggregate Functions
  - `COUNT()`
  - `SUM()`
  - `AVG()`
- `GROUP BY`
- `HAVING`
- `INNER JOIN`
- `LEFT JOIN`
- Subqueries
- `COALESCE()`
- Window Functions
  - `RANK()`
  - `DENSE_RANK()`
  - `ROW_NUMBER()`
  - `LAG()`
- Common Table Expressions (CTEs)

---

## 📊 Business Questions Solved

This project answers several real-world business questions, including:

- Find books belonging to a specific genre.
- Retrieve recently published books.
- Calculate total books currently in stock.
- Identify the highest and lowest priced books.
- Calculate total revenue generated.
- Find the most frequently ordered books.
- Identify customers with multiple purchases.
- Find the highest spending customers.
- Calculate remaining inventory after sales.
- Find books that have never been ordered.
- Find customers who have never placed an order.
- Rank customers based on total spending.
- Calculate running revenue over time.
- Identify the highest revenue-generating book in each genre.

---

## 📁 Repository Structure

```text
BookStore-SQL-Analytics/
│
├── BookStore_SQL_Analytics.sql
├── Books.csv
├── Customers.csv
├── Orders.csv
└── README.md
```

---

## 🚀 Getting Started

### 1. Install PostgreSQL

Download and install PostgreSQL on your system.

### 2. Create a Database

Create a new PostgreSQL database.

### 3. Execute the SQL Script

Run the `BookStore_SQL_Analytics.sql` file to create the required tables.

### 4. Import the Datasets

Import the CSV files using the `COPY` statements provided in the SQL script.

### 5. Run the Queries

Execute the SQL queries to explore insights and answer business questions.

---

## 💡 Skills Demonstrated

- PostgreSQL
- SQL
- Relational Database Design
- Data Cleaning
- Data Analysis
- Joins
- Aggregate Functions
- Window Functions
- Common Table Expressions (CTEs)
- Business Problem Solving

---

## 👨‍💻 Author

**Hemanth Chowdary**

GitHub: https://github.com/hemanthchowdary910