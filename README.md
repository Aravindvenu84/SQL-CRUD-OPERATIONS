# SQL CRUD Operations Using PostgreSQL

---

# Table of Contents

1. Introduction
2. Database Setup
3. Creating a Table
4. Inserting Sample Data
5. CRUD Operations
6. CRUD Query Examples
7. Screenshots Section
8. Explanation of CRUD Operations
9. Conclusion
10. References

---

# Introduction

This project demonstrates basic SQL database operations using PostgreSQL.

The project includes:
- Setting up a SQL database
- Creating a table
- Inserting sample data
- Performing CRUD operations
- Writing SQL queries
- Displaying query results

CRUD stands for:
- Create
- Read
- Update
- Delete

These are the four basic operations used in database management systems.

---

# Database Setup

## Database Used

- PostgreSQL

## Tools Used

- PostgreSQL
- pgAdmin / psql terminal
- Ubuntu Linux

## Create Database

```sql
CREATE DATABASE student_db;
```

## Connect to Database

```sql
\\c student_db
```

---

# Creating a Table

## Student Table Structure

The following SQL query creates a table named `students`.

```sql
CREATE TABLE students (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    course VARCHAR(100)
);
```

---

# Insert Sample Data

The following query inserts sample records into the table.

```sql
INSERT INTO students (name, age, course)
VALUES
('Arjun', 20, 'Computer Science'),
('Anjali', 22, 'Cyber Security'),
('Rahul', 21, 'Data Science');
```

---

# CRUD Operations

CRUD operations are the four basic operations performed on a database.

| Operation | Description |
|---|---|
| Create | Insert new records |
| Read | Retrieve records |
| Update | Modify existing records |
| Delete | Remove records |

---

# 1. CREATE Operation

## Description

The CREATE operation inserts new data into the database table.

## SQL Query

```sql
INSERT INTO students (name, age, course)
VALUES ('Meera', 23, 'Artificial Intelligence');
```

## Expected Result

A new row is added to the `students` table.

---

# Screenshot Placeholder — CREATE Operation


 <img width="816" height="503" alt="Screenshot from 2026-05-29 12-31-40" src="https://github.com/user-attachments/assets/61ee2c03-7853-4660-9562-52e4b244cf2e" />
 


---

# 2. READ Operation

## Description

The READ operation retrieves data from the database using the `SELECT` statement.

## SQL Query

```sql
SELECT * FROM students;
```

## Expected Result

Displays all records stored in the `students` table.

---

# Screenshot Placeholder — READ Operation

```text
[ ADD SCREENSHOT OF SELECT QUERY RESULT HERE ]
```

---

# 3. UPDATE Operation

## Description

The UPDATE operation modifies existing data in the table.

## SQL Query

```sql
UPDATE students
SET course = 'Machine Learning'
WHERE name = 'Rahul';
```

## Expected Result

The course of Rahul is updated to `Machine Learning`.

---

# Screenshot Placeholder — UPDATE Operation

```text
[ ADD SCREENSHOT OF UPDATE QUERY RESULT HERE ]
```

---

# 4. DELETE Operation

## Description

The DELETE operation removes records from the table.

## SQL Query

```sql
DELETE FROM students
WHERE name = 'Anjali';
```

## Expected Result

The record containing `Anjali` is removed from the table.

---

# Screenshot Placeholder — DELETE Operation

```text
[ ADD SCREENSHOT OF DELETE QUERY RESULT HERE ]
```

---

# Display Final Table Data

## SQL Query

```sql
SELECT * FROM students;
```

## Expected Result

Displays the remaining records after all CRUD operations.

---

# Screenshot Placeholder — Final Table

```text
[ ADD FINAL TABLE SCREENSHOT HERE ]
```

---

# CRUD Query Summary

## CREATE

```sql
INSERT INTO students (name, age, course)
VALUES ('Meera', 23, 'Artificial Intelligence');
```

---

## READ

```sql
SELECT * FROM students;
```

---

## UPDATE

```sql
UPDATE students
SET course = 'Machine Learning'
WHERE name = 'Rahul';
```

---

## DELETE

```sql
DELETE FROM students
WHERE name = 'Anjali';
```

---

# Explanation of CRUD Operations in PostgreSQL

## CREATE

The CREATE operation is used to insert new records into a database table using the `INSERT INTO` statement.

Example:
```sql
INSERT INTO students (name, age, course)
VALUES ('Arjun', 20, 'Computer Science');
```

This adds a new row to the table.

---

## READ

The READ operation retrieves stored information using the `SELECT` statement.

Example:
```sql
SELECT * FROM students;
```

This displays all rows and columns from the table.

---

## UPDATE

The UPDATE operation modifies existing records in the database.

Example:
```sql
UPDATE students
SET course = 'Machine Learning'
WHERE name = 'Rahul';
```

This changes existing values in selected rows.

---

## DELETE

The DELETE operation removes records from the table.

Example:
```sql
DELETE FROM students
WHERE name = 'Anjali';
```

This permanently deletes matching rows.

---

# Conclusion

This project demonstrated how CRUD operations work in PostgreSQL using SQL queries.

The following tasks were completed:
- Created a database
- Created a table
- Inserted sample data
- Performed Create, Read, Update, and Delete operations
- Displayed query results

CRUD operations are essential for:
- Web applications
- APIs
- Data management systems
- Enterprise software
- Database-driven applications

Understanding CRUD operations is fundamental for backend development and database management.

---

# References

- https://www.postgresql.org/
- https://www.w3schools.com/sql/
- https://www.geeksforgeeks.org/sql-tutorial/
- https://www.postgresqltutorial.com/
