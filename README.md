# PostgreSQL Queries - Patika.dev ASP.NET Core Assignment

This repository contains SQL queries related to the PostgreSQL database as part of the assignment for the Patika.dev ASP.NET Core course. The queries are designed to perform various operations on the `film` and `actor` tables of a sample database.

## Queries Overview

### 1. Retrieve all columns from the `film` table where the `replacement_cost` is between 12.99 and 16.99
```sql
SELECT * FROM film 
WHERE replacement_cost BETWEEN 12.99 AND 16.99;
```
This query returns all columns from the film table for rows where the replacement_cost is greater than or equal to 12.99 and less than 16.99 using the BETWEEN - AND operator.

### 2. Retrieve first_name and last_name columns from the actor table where the first_name is 'Penelope', 'Nick', or 'Ed'
```sql

SELECT first_name, last_name FROM actor 
WHERE first_name IN('Penelope','Nick','Ed');
```
This query selects and displays the first_name and last_name columns from the actor table for rows where the first_name matches one of the specified values using the IN operator.

### 3. Retrieve all columns from the film table where the rental_rate is 0.99, 2.99, or 4.99, and the replacement_cost is 12.99, 15.99, or 28.99
```sql

SELECT * FROM film 
WHERE rental_rate IN(0.99, 2.99, 4.99)
AND replacement_cost IN(12.99, 15.99, 28.99);
```
This query returns all columns from the film table for rows where the rental_rate is one of the specified values and the replacement_cost is also one of the specified values using the IN operator.
