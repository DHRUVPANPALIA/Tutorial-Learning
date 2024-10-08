# SQL Self Join: User-Admin Example

## Lesson Overview

In this lesson, we explore how to solve the user-admin problem using a self join. Self joins can be complex but are a powerful tool for comparing rows within the same table. This example demonstrates a practical application of self joins to match users with their respective admins.

## Key Concepts

- **Self Join**: A self join is a join where a table is joined with itself. It’s useful for comparing rows within the same table.
- **Primary Key**: In the user table, `user_id` is the primary key.
- **Foreign Key**: `admin_id` in the user table references `user_id` of another user, indicating the admin relationship.

## Steps to Solve the Problem

1. **Base Query**:
   - Start with a basic query to select all data from the `users` table:
     ```sql
     SELECT * FROM users;
     ```
   - The `user_id` is the primary key, and `admin_id` is a foreign key referencing another `user_id`.

2. **Initial Self Join**:
   - Perform a self join on the `users` table to see how it works:
     ```sql
     SELECT 
        users, admin 
     FROM 
        users
     LEFT JOIN 
        users as admin
     ON 
        user.userid = admin.userid;
     ```
   - This query shows two copies of the dataset side by side but doesn’t answer the business question.

3. **Join on Admin ID**:
   - Modify the join to connect the `admin_id` of the first table to the `user_id` of the second table:
     ```sql
     SELECT 
        users, admin 
     FROM 
        users
     LEFT JOIN 
        users as admin
     ON 
        user.adminid = admin.userid;   
     ```
   - This query links each user to their corresponding admin.


### Final Output

The result is a list showing each user's name alongside their admin’s name. This makes it easy to understand the relationships between users and admins.

## Conclusion

Self joins are a powerful tool for working with hierarchical data within the same table. By following these steps, you can effectively link related records and generate meaningful reports.

---

*This summary outlines the process of using a self join to solve the user-admin problem and provides a clear example of the SQL queries involved.*
