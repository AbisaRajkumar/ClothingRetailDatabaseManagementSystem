# 🛍️ Clothing Retail Store Database Management System

A fully normalized **BCNF-compliant database management system** for a multi-store clothing retail chain, complete with **SQL implementation**, **advanced queries**, and a **Java Swing GUI** connected to an Oracle database via JDBC.

---
---

## 👥 Authors

- Saloni Patel  
- Abisa Rajkumar  
- Immanuel Gnanaseelan  

---

## 📌 Project Overview

This project models the core operations of a clothing retail business, including:

- Customer and VIP management  
- Store and employee tracking  
- Inventory control across multiple locations  
- Order processing (online, in-store, pickup)  
- Discount and promotion handling  
- Analytical and advanced SQL queries  

The system was designed, normalized (up to **BCNF**), populated with sample data, and queried using **Oracle SQL**, with an optional **Java-based GUI** for interaction.

---

## 🧱 Technologies Used

- **Database:** Oracle SQL  
- **Programming Language:** Java  
- **GUI:** Java Swing  
- **Connectivity:** JDBC (ojdbc8)  
- **Concepts:**  
  - ER Modeling  
  - Functional Dependencies  
  - 3NF & BCNF Normalization  
  - Views, Joins, Subqueries  
  - Window Functions & Advanced SQL  

---

## 🗂️ Database Schema

### Core Tables
- `STORE`
- `CUSTOMER`
- `EMPLOYEE`
- `PRODUCT`
- `INVENTORY`
- `ORDERS`
- `ORDER_ITEM`
- `DISCOUNTS`

### Key Features
- Composite primary keys for inventory tracking  
- Foreign key constraints with cascading deletes  
- Data validation using `CHECK` constraints  
- Unique constraints for emails and phone numbers  

The final schema is **fully normalized to BCNF**, eliminating redundancy and ensuring data integrity.

---

## 🔍 Sample Queries Implemented

- Top customers by total spend and VIP tier  
- Employees whose average sales exceed store averages  
- Store-level revenue statistics (AVG, SUM, STDDEV)  
- Customers who ordered in-store but never online  
- Orders with active discounts  
- Combined employee & customer directory  

Views such as:
- `v_customer_spend`
- `v_open_stores`
- `v_recent_customers_2025`

---

## 🖥️ GUI Application (Java Swing)

A desktop GUI was built to interact with the database.

### Features
- Create & drop BCNF tables  
- Populate tables with sample data  
- View all tables  
- Search by primary key  
- Update and delete records  
- Run 5 advanced analytical queries  

### Requirements
- **Java JDK 21+**
- `ojdbc8.jar`
- Oracle database credentials

### How to Run
```bash
javac -cp ".;ojdbc8.jar" A9GUI.java
java -cp ".;ojdbc8.jar" A9GUI

```
---

## 📊 Data Integrity & Normalization

- Functional dependencies defined for each table  
- Decomposition performed where normalization violations existed  
- Inventory and Orders tables redesigned for **BCNF compliance**  
- Clear separation between **transactional data** (Orders, Order_Item) and  
  **reference data** (Store, Product, Customer, Employee)

---

## 📎 Notes

This project was developed as part of an academic database systems course and demonstrates:

- Real-world relational database design  
- Advanced SQL (joins, views, subqueries, window functions)  
- Database normalization (3NF --> BCNF)  
- GUI integration using Java Swing and JDBC



