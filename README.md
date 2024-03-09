# sql_begin
Certainly! Here's the revised introduction with added emojis:

---

# SQL Queries Guide for Beginners

👋 Welcome to the SQL Queries Guide for Beginners! 🎉 In this guide, you'll find simple and illustrative examples of common SQL queries using a hypothetical `students` table.

## Table of Contents

1. [Introduction](#introduction)
2. [Queries](#queries)
    - [SELECT](#select)
    - [CREATE](#create)
    - [DELETE](#delete)
    - [UPDATE](#update)
    - [AND, OR](#and-or)
    - [LIKE and Wildcards](#like-and-wildcards)
    - [LIMIT](#limit)
    - [Aggregate Functions](#aggregate-functions)

## Introduction

SQL (Structured Query Language) is a powerful tool used for managing and manipulating relational databases. It allows you to perform various operations such as querying, updating, and deleting data.

In this guide, we'll use a hypothetical `students` table to demonstrate how to write SQL queries for common tasks. Let's dive in! 💻✨

## Queries

### SELECT

The `SELECT` statement is used to retrieve data from one or more tables. Here's an example:

```sql
SELECT * FROM students;
```

This query selects all columns (`*`) from the `students` table.

### CREATE

The `CREATE TABLE` statement is used to create a new table. Here's an example:

```sql
CREATE TABLE students (
    ID INT AUTO_INCREMENT PRIMARY KEY,
    First_name VARCHAR(20) NOT NULL,
    Last_name VARCHAR(30) NOT NULL,
    Age INT NOT NULL
);
```

This query creates a new table named `students` with columns for `ID`, `First_name`, `Last_name`, and `Age`.

### DELETE

The `DELETE` statement is used to delete rows from a table. Here's an example:

```sql
DELETE FROM students WHERE ID = 1;
```

This query deletes the student with `ID` equal to 1 from the `students` table.

### UPDATE

The `UPDATE` statement is used to modify existing records in a table. Here's an example:

```sql
UPDATE students SET Age = 20 WHERE First_name = 'John';
```

This query updates the `Age` of the student named 'John' to 20.

### AND, OR

The `AND` and `OR` operators are used to combine multiple conditions in a `WHERE` clause. Here's an example:

```sql
SELECT * FROM students WHERE Age > 18 AND Last_name = 'Doe';
```

This query selects students who are older than 18 and have the last name 'Doe'.

### LIKE and Wildcards

The `LIKE` operator is used to search for a specified pattern in a column. Wildcards (`%`) can be used to represent zero or more characters. Here's an example:

```sql
SELECT * FROM students WHERE First_name LIKE 'J%';
```

This query selects students whose first names start with the letter 'J'.

### LIMIT

The `LIMIT` clause is used to limit the number of rows returned by a query. Here's an example:

```sql
SELECT * FROM students LIMIT 10;
```

This query selects the first 10 rows from the `students` table.

### Aggregate Functions

Aggregate functions perform a calculation on a set of values and return a single value. Here are examples of some common aggregate functions:

- `COUNT`: Counts the number of rows.
- `AVG`: Calculates the average value.
- `SUM`: Calculates the sum of values.
- `MIN`: Returns the minimum value.
- `MAX`: Returns the maximum value.

```sql
SELECT COUNT(*) FROM students;
SELECT AVG(Age) FROM students;
```

The first query counts the number of students, while the second query calculates the average age of students.
