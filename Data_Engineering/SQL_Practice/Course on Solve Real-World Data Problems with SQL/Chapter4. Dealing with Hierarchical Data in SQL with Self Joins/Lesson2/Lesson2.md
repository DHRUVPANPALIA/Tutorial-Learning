# SQL Self Join: User-Admin Example

## Lesson Overview

In this lesson, we explore how to solve the user-admin problem using a self join. Self joins can be complex but are a powerful tool for comparing rows within the same table. This example demonstrates a practical application of self joins to match users with their respective admins.

## Key Concepts

- **Self Join**: A self join is a join where a table is joined with itself. It’s useful for comparing rows within the same table.
- **Primary Key**: In the user table, `user_id` is the primary key.
- **Foreign Key**: `admin_id` in the user table references `user_id` of another user, indicating the admin relationship.

## Steps to Solve the Problem

1. **Base Query**: Start by selecting all columns from the `users` table:
   ```sql
   SELECT * FROM users;
