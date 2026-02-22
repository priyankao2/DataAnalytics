# 🔹 Project 2: E-Commerce Data Management (SQL)

## 📌 Project Overview

This project demonstrates database creation, structured data storage,
and business data analysis using SQL. The system manages customers,
products, and orders while generating insights like revenue and
top-selling products.

------------------------------------------------------------------------

## 🏗 Step 1: Database Creation

``` sql
CREATE DATABASE ecommerce_db;
```

------------------------------------------------------------------------

## 🏗 Step 2: Table Creation

### Customers Table

``` sql
CREATE TABLE customers (
    customer_id SERIAL PRIMARY KEY,
    customer_name VARCHAR(100),
    city VARCHAR(50),
    email VARCHAR(100)
);
```

### Products Table

``` sql
CREATE TABLE products (
    product_id SERIAL PRIMARY KEY,
    product_name VARCHAR(100),
    category VARCHAR(50),
    price DECIMAL(10,2)
);
```

### Orders Table

``` sql
CREATE TABLE orders (
    order_id SERIAL PRIMARY KEY,
    customer_id INT REFERENCES customers(customer_id),
    product_id INT REFERENCES products(product_id),
    quantity INT,
    order_date DATE
);
```

------------------------------------------------------------------------

## 📥 Step 3: Insert Sample Data

``` sql
INSERT INTO customers (customer_name, city, email) VALUES
('Rahul Sharma', 'Kolkata', 'rahul@gmail.com'),
('Sneha Das', 'Delhi', 'sneha@gmail.com'),
('Amit Roy', 'Mumbai', 'amit@gmail.com');
```

``` sql
INSERT INTO products (product_name, category, price) VALUES
('Laptop', 'Electronics', 50000),
('Headphones', 'Electronics', 2000),
('Book', 'Education', 500);
```

``` sql
INSERT INTO orders (customer_id, product_id, quantity, order_date) VALUES
(1, 1, 1, '2026-01-01'),
(2, 2, 2, '2026-01-02'),
(1, 3, 3, '2026-01-05'),
(3, 1, 1, '2026-01-10');
```

------------------------------------------------------------------------

## 📊 Step 4: Business Analysis Queries

### ✅ Total Sales Per Product

``` sql
SELECT p.product_name,
       SUM(o.quantity * p.price) AS total_sales
FROM orders o
JOIN products p ON o.product_id = p.product_id
GROUP BY p.product_name;
```

### ✅ Top Selling Product

``` sql
SELECT p.product_name,
       SUM(o.quantity) AS total_quantity
FROM orders o
JOIN products p ON o.product_id = p.product_id
GROUP BY p.product_name
ORDER BY total_quantity DESC
LIMIT 1;
```

### ✅ Total Revenue

``` sql
SELECT SUM(o.quantity * p.price) AS total_revenue
FROM orders o
JOIN products p ON o.product_id = p.product_id;
```

------------------------------------------------------------------------

## 🎯 Skills Demonstrated

-   Database Design\
-   SQL (SELECT, JOIN, GROUP BY, ORDER BY)\
-   Aggregation Functions\
-   Revenue & Sales Analysis\
-   Business Insights Generation

------------------------------------------------------------------------

# 🚀 Tools Used

-   Microsoft Excel\
-   PostgreSQL / MySQL\
-   SQL

------------------------------------------------------------------------

# 📌 Author

**Priyanka Gupta**\
Aspiring Data Analyst \| Skilled in Excel & SQL
