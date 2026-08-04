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