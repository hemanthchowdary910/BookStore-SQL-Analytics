\# Book Store Management System | PostgreSQL SQL Project



\## Project Overview



This project focuses on analyzing a bookstore database using PostgreSQL.



The goal of this project was to practice SQL by creating relational tables, importing CSV data, and writing queries to answer different business questions related to books, customers, orders, sales, and inventory.



The database contains information about available books, customers, and customer orders. The analysis includes basic data retrieval, sales calculations, customer analysis, inventory tracking, and revenue-based insights.



\---



\## Database Structure



The database consists of three connected tables:



\### Books



Stores information about the books available in the store.



Columns:



\* Book ID

\* Title

\* Author

\* Genre

\* Published Year

\* Price

\* Stock



\### Customers



Contains customer information.



Columns:



\* Customer ID

\* Name

\* Email

\* Phone

\* City

\* Country



\### Orders



Stores customer purchase information.



Columns:



\* Order ID

\* Customer ID

\* Book ID

\* Order Date

\* Quantity

\* Total Amount



\### Table Relationships



```

Customers

&#x20;   |

&#x20;   | 1 : Many

&#x20;   |

&#x20;Orders

&#x20;   |

&#x20;   | Many : 1

&#x20;   |

&#x20;Books

```



\---



\## Dataset Information



The project uses three CSV files:



\* Books.csv - Contains book details such as title, author, genre, price, and stock.

\* Customers.csv - Contains customer information.

\* Orders.csv - Contains order transactions and purchase details.



The data was imported into PostgreSQL using the `COPY` command.



\---



\## SQL Concepts Practiced



This project covers various PostgreSQL and SQL concepts:



\* Database and table creation

\* Primary keys and foreign keys

\* Data importing using COPY

\* Filtering data using WHERE

\* Sorting using ORDER BY

\* Aggregations using SUM, COUNT, and AVG

\* GROUP BY and HAVING clauses

\* INNER JOIN and LEFT JOIN

\* Subqueries

\* COALESCE function

\* Window functions:



&#x20; \* RANK()

&#x20; \* DENSE\_RANK()

&#x20; \* ROW\_NUMBER()

&#x20; \* LAG()

\* Common Table Expressions (CTEs)



\---



\## Business Questions Answered



Some of the analysis performed in this project includes:



\* Finding books from specific genres

\* Identifying recently published books

\* Calculating total available stock

\* Finding the highest and lowest priced books

\* Calculating total revenue generated from orders

\* Finding the most frequently ordered books

\* Identifying customers with multiple orders

\* Finding customers with the highest spending

\* Calculating remaining stock after completed orders

\* Finding books and customers with no associated orders

\* Ranking customers based on spending

\* Calculating running revenue over time

\* Finding the highest revenue-generating book in each genre



\---



\## Repository Structure



```

BookStore-SQL-Analytics/



│

├── BookStore\_SQL\_Project.sql

├── Books.csv

├── Customers.csv

├── Orders.csv

└── README.md

```



\---



\## How to Run This Project



1\. Install PostgreSQL.

2\. Create a new database.

3\. Run the SQL file to create tables and execute queries.

4\. Import the CSV files using the provided COPY statements.

5\. Execute the analysis queries to view results.



\---



\## Skills Demonstrated



\* PostgreSQL

\* SQL Query Writing

\* Relational Database Design

\* Data Analysis

\* Joins and Aggregations

\* Business Problem Solving



\---



\## Author



Hemanth Chowdary



GitHub:

https://github.com/hemanthchowdary910



