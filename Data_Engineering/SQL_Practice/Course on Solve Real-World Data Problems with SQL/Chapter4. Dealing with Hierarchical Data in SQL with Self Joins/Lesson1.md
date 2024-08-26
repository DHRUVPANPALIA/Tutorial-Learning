# SQL Practice Course

## Course Overview

This course is designed to enhance your SQL skills through hands-on practice and exercises. You'll learn the fundamentals of SQL and advance to more complex queries and database management tasks.

## Topics Covered

1. **Introduction to SQL**
   - Basic SQL Syntax
   - Data Types
   - Basic Query Structure

2. **Database Design**
   - Creating Tables
   - Primary and Foreign Keys
   - Normalization

3. **CRUD Operations**
   - `SELECT` Queries
   - `INSERT` Statements
   - `UPDATE` Statements
   - `DELETE` Statements

4. **Joins and Subqueries**
   - INNER JOIN
   - LEFT JOIN
   - RIGHT JOIN
   - FULL JOIN
   - Subqueries

5. **Advanced SQL**
   - Indexes
   - Transactions
   - Stored Procedures
   - Views

6. **Performance Optimization**
   - Query Optimization Techniques
   - Analyzing Execution Plans

## Setup Instructions

1. **Install SQL Database Software**:
   - [MySQL](https://dev.mysql.com/downloads/)
   - [PostgreSQL](https://www.postgresql.org/download/)
   - [SQLite](https://www.sqlite.org/download.html)

2. **Set Up Your Environment**:
   - Download and install an SQL client (e.g., MySQL Workbench, pgAdmin, DB Browser for SQLite).

3. **Create a Sample Database**:
   - Use the provided SQL script to set up the sample database.

   ```sql
   CREATE TABLE employees (
       id INT PRIMARY KEY,
       name VARCHAR(100),
       position VARCHAR(100),
       salary DECIMAL(10, 2)
   );
