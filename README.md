# Book Store Management System | PostgreSQL SQL Project

## Project Overview

This project focuses on analyzing a bookstore database using PostgreSQL.

The goal of this project was to practice SQL by creating relational tables, importing CSV data, and writing queries to answer different business questions related to books, customers, orders, sales, and inventory.

The database contains information about available books, customers, and customer orders. The analysis includes basic data retrieval, sales calculations, customer analysis, inventory tracking, and revenue-based insights.

---

## Database Structure

The database consists of three connected tables.

### Books

Stores information about the books available in the store.

Columns:
- Book ID
- Title
- Author
- Genre
- Published Year
- Price
- Stock

### Customers

Contains customer information.

Columns:
- Customer ID
- Name
- Email
- Phone
- City
- Country

### Orders

Stores customer purchase information.

Columns:
- Order ID
- Customer ID
- Book ID
- Order Date
- Quantity
- Total Amount

### Table Relationships

```text
Customers
    |
    | 1 : Many
    |
  Orders
    |
    | Many : 1
    |
  Books
```

- One customer can place multiple orders.
- One book can appear in multiple orders.

---

## Dataset Information

The project uses three CSV datasets:

- **Books.csv** - Contains book details such as title, author, genre, price, and stock.
- **Customers.csv** - Contains customer information.
- **Orders.csv** - Contains order transaction details.

The datasets were imported into PostgreSQL using the `COPY` command.

---

## SQL Concepts Practiced

The project demonstrates the following SQL concepts:

- Database and table creation
- Primary keys and foreign keys
- Data importing using `COPY`
- Filtering with `WHERE`
- Sorting with `ORDER BY`
- Aggregate functions:
  - `SUM()`
  - `COUNT()`
  - `AVG()`
- `GROUP BY` and `HAVING`
- `INNER JOIN`
- `LEFT JOIN`
- Subqueries
- `COALESCE()`
- Window Functions:
  - `RANK()`
  - `DENSE_RANK()`
  - `ROW_NUMBER()`
  - `LAG()`
- Common Table Expressions (CTEs)

---

## Analysis Performed

The project answers business questions such as:

- Finding books by genre
- Identifying recently published books
- Calculating total available stock
- Finding highest and lowest priced books
- Calculating total revenue generated
- Finding frequently ordered books
- Identifying customers with multiple orders
- Finding highest spending customers
- Calculating remaining stock after orders
- Finding books that were never ordered
- Finding customers with no orders
- Ranking customers based on spending
- Calculating running revenue over time
- Finding the highest revenue-generating book in each genre

---

## Repository Structure
BookStore-SQL-Analytics/

├── BookStore_SQL_Analytics.sql
├── Books.csv
├── Customers.csv
├── Orders.csv
└── README.md


---

## How to Run This Project

1. Install PostgreSQL.
2. Create a new database.
3. Execute the SQL file to create tables.
4. Import CSV files using the provided `COPY` statements.
5. Run the queries to view analysis results.

---

## Skills Demonstrated

- PostgreSQL
- SQL Query Writing
- Relational Database Design
- Data Analysis
- Joins and Aggregations
- Business Problem Solving

---

## Author

**Hemanth Chowdary**

GitHub:
https://github.com/hemanthchowdary910