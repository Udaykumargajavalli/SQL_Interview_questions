### 1. What is SQL?
SQL (Structured Query Language) is a standard language for accessing and manipulating relational databases. It is used to query, insert, update, and delete data, as well as to create and modify the structure of database systems.


---
### 2. What are the different types of SQL statements?

- DDL (Data Definition Language): CREATE, ALTER, DROP
- DML (Data Manipulation Language): SELECT, INSERT, UPDATE, DELETE
- DCL (Data Control Language): GRANT, REVOKE
- TCL (Transaction Control Language): COMMIT, ROLLBACK, SAVEPOINT
---
### 3. What is the difference between WHERE and HAVING?

- `WHERE` filters rows before grouping.
- `HAVING` filters groups after aggregation.

Example:
```sql
SELECT department, COUNT(*) 
FROM employees 
WHERE salary > 50000 
GROUP BY department 
HAVING COUNT(*) > 5;
```
---
### 4. What is a primary key?
A primary key is a field in a table which uniquely identifies each row/record in that table. Primary keys must contain unique values and cannot contain NULL values.

---
### 5. What is a foreign key?
A foreign key is a field (or collection of fields) in one table that uniquely identifies a row of another table. The foreign key is defined in a second table, but it refers to the primary key or a unique key in the first table.

---
### 6. What is a join?
A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

---
### 7. What are the different types of joins?
The different types of joins are INNER JOIN, LEFT JOIN (or LEFT OUTER JOIN), RIGHT JOIN (or RIGHT OUTER JOIN), and FULL JOIN (or FULL OUTER JOIN).

---
### 8. What is an index?
An index is a performance-tuning method of allowing faster retrieval of records from the table. An index creates an entry for each value and it will be faster to retrieve data.

---
### 9. What is normalization?
Normalization is the process of organizing data to minimize redundancy. Normalization usually involves dividing a database into two or more tables and defining relationships between the tables.

---
### 10. What is denormalization?
Denormalization is the process of attempting to optimize the read performance of a database by adding redundant data or by grouping data. It is the opposite of normalization.

---
### 11. What is a view?
A view is a virtual table based on the result-set of an SQL statement. It contains rows and columns, just like a real table. The fields in a view are fields from one or more real tables in the database.

---
### 12. What is a stored procedure?
A stored procedure is a prepared SQL code that you can save, so the code can be reused over and over again. You can also pass parameters to a stored procedure, so that the stored procedure can act based on the parameter value(s) that is passed.

---
### 13. What is a trigger?
A trigger is a set of SQL statements that automatically 'fires' or executes when certain events occur. Triggers are used to maintain the integrity of the information on the database.

---
### 14. What is a subquery?
A subquery is a query within another query. The outer query is called the main query, and the inner query is called the subquery. Subqueries are used to return data that will be used in the main query as a condition to further restrict the data to be retrieved.

---
### 15. What is a transaction?
A transaction is a sequence of one or more SQL operations treated as a unit. If one part of the transaction fails, the entire transaction fails, and the database state is left unchanged.

---
### 16. What is a constraint?
Constraints are used to specify rules for the data in a table. Constraints can be specified when the table is created (inside the CREATE TABLE statement) or after the table is created (inside the ALTER TABLE statement).

---
### 17. What is a unique constraint?
A unique constraint ensures that all values in a column are different. Both the UNIQUE and PRIMARY KEY constraints provide a guarantee for uniqueness for a column or set of columns.

---
### 18. What is a check constraint?
A check constraint is used to limit the value range that can be placed in a column. If you define a check constraint on a column, it will allow only certain values for this column.

---
### 19. What is a default constraint?
A default constraint is used to provide a default value for a column. The default value will be added to all new records if no other value is specified.

---
### 20. What is a composite key?
A composite key is a combination of two or more columns in a table that can be used to uniquely identify each row in the table.

---
### 21. What is a self join?
A self join is a regular join, but the table is joined with itself.

---
### 22. What is a cross join?
A cross join is a Cartesian product of the two tables involved in the join. The result set will contain all combinations of rows from the two tables.

---
### 23. What is a union?
The UNION operator is used to combine the result set of two or more SELECT statements. Each SELECT statement within the UNION must have the same number of columns in the result sets with similar data types.

---
### 24. What is the difference between UNION and UNION ALL?
The UNION operator selects only distinct values by default. The UNION ALL operator selects all values, including duplicates.

---
### 25. What is a cursor?
A cursor is a database object that allows you to retrieve each row from a result set one at a time. Cursors are used when the user needs to update records in a database table one row at a time.

---
### 26. What is an alias?
An alias is a temporary name given to a table or column for the purpose of a particular SQL query. Aliases are created to make table or column names more readable.

---
### 27. What is a case statement?
The CASE statement is SQL's way of handling if/then logic. It allows you to perform conditional logic in a SQL query.

---
### 28. What is the difference between DELETE and TRUNCATE?
DELETE is a DML command and removes rows one at a time and records an entry in the transaction log for each deleted row. TRUNCATE is a DDL command and removes all rows from a table without logging the individual row deletions.

---
### 39. What is the difference between DROP and TRUNCATE?
DROP is a DDL command that removes a table from the database. TRUNCATE is a DDL command that removes all rows from a table but does not remove the table itself.

---
### 40. What is the difference between CHAR and VARCHAR?
CHAR is a fixed-length data type, while VARCHAR is a variable-length data type. CHAR will always use the same amount of storage space, while VARCHAR will use only the amount of space needed to store the data.

---
### 41. What is the difference between IN and EXISTS?
The IN operator is used to compare a value to a list of values, while the EXISTS operator is used to check the existence of a result of a subquery.

---
### 42. What is the difference between a clustered and a non-clustered index?
A clustered index determines the physical order of data in a table and is used to improve the performance of data retrieval. A non-clustered index does not alter the physical order of data and is used to create a logical order for data rows.

---
### 43. What is the difference between a primary key and a unique key?
A primary key uniquely identifies each row in a table and cannot contain NULL values. A unique key also ensures the uniqueness of the column but can contain NULL values.

---
### 44. What is the difference between a left join and a right join?
A left join returns all rows from the left table and the matched rows from the right table. A right join returns all rows from the right table and the matched rows from the left table.

---
### 45. What is the difference between a full join and an inner join?
A full join returns all rows when there is a match in either table. An inner join returns only the rows that have matching values in both tables.

---
### 46. What is the difference between a subquery and a join?
A subquery is a query within another query, while a join is used to combine rows from two or more tables based on a related column between them.

---
### 47. What is the difference between a stored procedure and a function?
A stored procedure is a set of SQL statements that can perform a specific task, while a function is a set of SQL statements that can return a single value. Functions can be used in SQL statements, while stored procedures cannot.

---
### 48. What is the difference between a view and a table?
A view is a virtual table based on the result-set of an SQL statement, while a table is a collection of related data held in a structured format within a database.

---
### 49. What are the properties of a transaction in sql?
In SQL, the properties of a transaction are defined by the ACID principle, which ensures the reliability and integrity of database operations.

**1. Atomicity**

Definition: Atomicity ensures that a transaction is treated as a single, indivisible unit of work. Either all operations within the transaction are completed successfully, or none are.
Example: If you're transferring money from Account A to Account B, both the debit from A and the credit to B must succeed. If one fails, the entire transaction is rolled back.

**2. Consistency**

Definition: Consistency ensures that a transaction brings the database from one valid state to another, maintaining all predefined rules, such as constraints, cascades, and triggers.
Example: If a table has a constraint that a column must be unique, a transaction that violates this rule will not be allowed to commit.

**3. Isolation**

Definition: Isolation ensures that concurrent transactions do not interfere with each other. The intermediate state of a transaction is invisible to other transactions.
Example: If two users are booking the last seat on a flight simultaneously, isolation ensures that only one booking is confirmed, avoiding double-booking.

**4. Durability**

Definition: Durability guarantees that once a transaction is committed, its changes are permanent, even in the event of a system failure.
Example: After a successful transaction that updates a customer’s address, the new address remains saved even if the system crashes immediately afterward.

---
### 50. What is the difference between a temporary table and a table variable?
A temporary table is a table that is created and exists temporarily on the database server, while a table variable is a variable that holds a table and is created and exists temporarily in the memory.

---
### 51. What is the difference between a correlated subquery and a non-correlated subquery?
A correlated subquery is a subquery that references columns from the outer query, while a non-correlated subquery is a subquery that does not reference columns from the outer query.

---
### 52. Query to find Nth salary of employee data

```sql
SELECT DISTINCT salary
FROM Employee
ORDER BY salary DESC
LIMIT 1 OFFSET N-1;
```
---
### 53. Difference between rank and dense rank. Explain with an example
Both are window functions used to assign a ranking to rows based on a specific column's values. The key difference is how they handle ties (duplicate values).

`RANK()` and `DENSE_RANK()` are SQL window functions used to assign ranks to rows based on the order of a specified column. They are often used in analytical queries like finding top-N results or ranking employees by salary.

### 🔍 Key Differences

| Feature       | `RANK()`                          | `DENSE_RANK()`                     |
|---------------|-----------------------------------|------------------------------------|
| Tie Handling  | Same rank for ties, **skips** next rank(s) | Same rank for ties, **no skipping** |
| Gaps in Rank? | ✅ Yes                             | ❌ No                               |

### 📋 Sample Data

Let's assume we have the following `Employee` table:

```sql
| EmpID | Salary |
|-------|--------|
| 1     | 5000   |
| 2     | 6000   |
| 3     | 6000   |
| 4     | 7000   |

🏷 Example: Using RANK()
SELECT EmpID, Salary, RANK() OVER (ORDER BY Salary DESC) AS rank
FROM Employee;

| EmpID | Salary | Rank |
| ----- | ------ | ---- |
| 4     | 7000   | 1    |
| 2     | 6000   | 2    |
| 3     | 6000   | 2    |
| 1     | 5000   | 4    |

✅ Notice how rank 3 is skipped due to the tie on salary.

🏷 Example: Using DENSE_RANK()
SELECT EmpID, Salary, DENSE_RANK() OVER (ORDER BY Salary DESC) AS dense_rank
FROM Employee;

| EmpID | Salary | Dense\_Rank |
| ----- | ------ | ----------- |
| 4     | 7000   | 1           |
| 2     | 6000   | 2           |
| 3     | 6000   | 2           |
| 1     | 5000   | 3           |

🚫 No ranks are skipped, even with duplicate values.
```
✅ Summary
* Use RANK() if you want to preserve gaps when values are tied.
* Use DENSE_RANK() when you want consecutive ranks regardless of ties.
---
### 54. Different Types of SQL Joins

SQL joins are used to combine rows from two or more tables based on a related column.

### 1. ✅ INNER JOIN

Returns only matching rows between tables.

```sql
SELECT *
FROM Employees e
INNER JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Keeps only rows where DeptID matches in both tables.

### 2. ⬅️ LEFT JOIN (or LEFT OUTER JOIN)

Returns all rows from the left table, and matching rows from the right.
```sql
SELECT *
FROM Employees e
LEFT JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Unmatched right-side values are returned as NULL.

### 3. ➡️ RIGHT JOIN (or RIGHT OUTER JOIN)
Returns all rows from the right table, and matching rows from the left.
```sql
SELECT *
FROM Employees e
RIGHT JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Unmatched left-side values are returned as NULL.

4. 🔄 FULL OUTER JOIN
Returns all rows when there is a match in either table.
```sql
SELECT *
FROM Employees e
FULL OUTER JOIN Departments d ON e.DeptID = d.ID;
```
🔍 Combines results of LEFT and RIGHT joins. Missing matches are shown as NULL.

5. ❌ CROSS JOIN
Returns Cartesian product — all possible combinations of rows.
```sql
SELECT *
FROM Employees
CROSS JOIN Departments;
```
🔍 Use with caution! Rows = A × B (can be huge).

📌 Summary Table
| Join Type       | Description                                | NULLs Possible? |
| --------------- | ------------------------------------------ | --------------- |
| INNER JOIN      | Matching rows from both tables             | ❌               |
| LEFT JOIN       | All from left + matched from right         | ✅ Right side    |
| RIGHT JOIN      | All from right + matched from left         | ✅ Left side     |
| FULL OUTER JOIN | All rows from both, matched where possible | ✅ Both sides    |
| CROSS JOIN      | All combinations (Cartesian product)       | ❌               |
---

### 55. Minimum and Maximum Rows Returned by SQL Joins

Understanding how many rows a SQL join can return is crucial for query optimization and avoiding unexpected results.

### 🔍 Join Behavior Summary

| Join Type          | Minimum Rows Returned                       | Maximum Rows Returned                      |
|--------------------|---------------------------------------------|--------------------------------------------|
| **INNER JOIN**     | `0` (if no matches exist in either table)   | `min(#rows in A, #rows in B)`              |
| **LEFT JOIN**      | `#rows in A`                                | `#rows in A` (with possible NULLs from B)  |
| **RIGHT JOIN**     | `#rows in B`                                | `#rows in B` (with possible NULLs from A)  |
| **FULL OUTER JOIN**| `max(#rows in A, #rows in B)`               | `#rows in A + #rows in B`                  |
| **CROSS JOIN**     | `#rows in A × #rows in B`                   | `#rows in A × #rows in B`                  |

> ✅ **Note**:  
> - `A` = Left Table  
> - `B` = Right Table  
> - `NULLs` appear when there's no match in non-preserved tables.

### 📘 Example Scenario

Let’s say:

- Table A (Employees): 3 rows  
- Table B (Departments): 2 rows

Then:

| Join Type          | Example Row Count Returned          |
|--------------------|-------------------------------------|
| **INNER JOIN**     | 0 to 2 (depends on matching `DeptID`)|
| **LEFT JOIN**      | 3 (always all from Employees)        |
| **RIGHT JOIN**     | 2 (always all from Departments)      |
| **FULL OUTER JOIN**| 3 to 5 (all unmatched + matched rows)|
| **CROSS JOIN**     | 3 × 2 = 6                            |


### 🔄 Join Behavior Explained

- **INNER JOIN**: Only rows with matching keys in both tables.
- **LEFT JOIN**: All rows from the left table, with NULLs where there's no match on the right.
- **RIGHT JOIN**: All rows from the right table, with NULLs where there's no match on the left.
- **FULL OUTER JOIN**: All rows from both sides, with NULLs for unmatched columns.
- **CROSS JOIN**: Every row in A joins with every row in B (Cartesian product).

📌 Useful for estimating result size and understanding query performance!

---

### 56. what are some optimization that you can do for SQL?

Optimizing SQL queries is crucial for improving the performance, scalability, and responsiveness of your database-driven applications. Below are some best practices and techniques to help you write efficient SQL:

#### ✅ 1. **Use Proper Indexing**
- Create indexes on columns used in `WHERE`, `JOIN`, `ORDER BY`, and `GROUP BY` clauses.
- Avoid over-indexing, which can slow down `INSERT`, `UPDATE`, and `DELETE` operations.
- Use **composite indexes** when filtering on multiple columns.

#### ✅ 2. **Avoid SELECT ***  
- Always specify only the columns you need.
- Reduces I/O and improves performance, especially with large tables.

#### ✅ 3. **Use Joins Efficiently**
- Prefer `INNER JOIN` over `OUTER JOIN` when possible.
- Ensure join columns are indexed.
- Avoid joining unnecessary tables.

#### ✅ 4. **Filter Early with WHERE**
- Use `WHERE` clauses to reduce the number of rows as early as possible.
- Avoid functions on columns in `WHERE` (e.g., `WHERE YEAR(date) = 2023`) as they prevent index usage.

#### ✅ 5. **Limit Result Sets**
- Use `LIMIT` or `TOP` to restrict the number of rows returned.
- Useful for pagination and reducing load on the client and server.

#### ✅ 6. **Optimize Subqueries**
- Replace correlated subqueries with `JOIN`s or `WITH` (CTEs) when possible.
- Use `EXISTS` instead of `IN` for better performance in many cases.

#### ✅ 7. **Use EXPLAIN / ANALYZE**
- Analyze query execution plans to identify bottlenecks.
- Helps understand how indexes and joins are being used.

#### ✅ 8. **Avoid Wildcards in LIKE**
- Avoid leading wildcards (e.g., `LIKE '%term'`) as they prevent index usage.
- Consider full-text search for complex text queries.

#### ✅ 9. **Batch Updates and Inserts**
- Use bulk operations instead of row-by-row processing.
- Reduces transaction overhead and improves throughput.

#### ✅ 10. **Keep Transactions Short**
- Long transactions can lock resources and reduce concurrency.
- Commit or rollback as soon as possible.

---

### 57. Difference Between UNION and UNION ALL in SQL? which one you use and at what situations?

#### UNION vs UNION ALL

In SQL, both `UNION` and `UNION ALL` are used to combine the results of two or more `SELECT` queries. However, they have some key differences:

#### ✅ UNION

- **Removes Duplicates**: Returns only distinct rows from the combined result set.
- **Performance**: Slower than `UNION ALL` because it performs a distinct sort operation.
- **Use Case**: When you need a clean, non-redundant list of results.

#### Example:
```sql
SELECT city FROM customers
UNION
SELECT city FROM suppliers;
```
#### ✅ UNION ALL
* Keeps Duplicates: Returns all rows, including duplicates.
* Performance: Faster than UNION because it skips the duplicate check.
* Use Case: When duplicates are acceptable or needed for analysis.
  
#### Example:
```sql
SELECT city FROM customers
UNION ALL
SELECT city FROM suppliers;
```

🧠 When to Use What?
| Use Case                          | Recommended |
|----------------------------------|-------------|
| You need unique results          | `UNION`     |
| You want better performance      | `UNION ALL` |
| You want to preserve duplicates  | `UNION ALL` |
| You are aggregating or counting  | `UNION ALL` (then filter/aggregate) |

---

### 58. what is CTE and syntax, how many ctes you can write in sql query?

#### What is a CTE?

A **Common Table Expression (CTE)** is a temporary result set in SQL that can be referenced within another SQL query. CTEs help improve the readability and modularity of complex queries.

## Syntax

```sql
WITH cte_name AS (
    SELECT column1, column2
    FROM some_table
    WHERE condition
)
SELECT *
FROM cte_name;
```

#### How many CTEs can you write in a SQL query?
There is no strict limit on the number of CTEs you can define in a query — it's constrained by the SQL engine (e.g., PostgreSQL, SQL Server, MySQL) and the available system memory. In practice, many CTEs can be used as long as the query remains manageable and performs well.

📌 Summary
* WITH defines a CTE.
* Improves clarity of complex queries.
* Supports multiple CTEs in one query.
* No strict limit — use as needed with performance in mind.

---

### 59. Differences between cte and subquery?
| Feature               | CTE (Common Table Expression)                                        | Subquery                                                   |
| --------------------- | -------------------------------------------------------------------- | ---------------------------------------------------------- |
| **Definition**        | A temporary result set defined using `WITH` at the start of a query  | A nested query inside `SELECT`, `FROM`, or `WHERE` clauses |
| **Readability**       | More readable for complex queries with multiple steps                | Can become hard to read when deeply nested                 |
| **Reusability**       | Can be referenced multiple times within the main query               | Cannot be reused; needs to be repeated                     |
| **Recursion Support** | Supports recursion (especially for hierarchical data)                | Does not support recursion                                 |
| **Performance**       | Often optimized similarly to subqueries; readability is the main win | Slightly more performant in simple cases                   |
| **Scope**             | Available only to the query immediately following it                 | Limited to the part of the query where it’s used           |

🧠 Summary:
* Use CTEs when your query is complex, needs recursion, or has reusable logic.
* Use subqueries for quick, simple logic that's only needed once.
---

### 60. Explain about self join vs subquery
#### ✅ Self Join
A self join is a join where a table is joined to itself. It's used when you want to compare rows within the same table.

##### 📌 Use Case:
Find relationships between rows in the same table, such as manager-employee, product-category, or friend connections.

#### ✅ Subquery
A subquery is a query embedded inside another query. It can return a single value (scalar), a row, or a table, and can be used in SELECT, FROM, or WHERE clauses.

###### 📌 Use Case:
Use when you want to filter, calculate, or retrieve a value based on another query result.

---

### 61. Tell me a situation where you used or we can use CTE in sql?
There can be multiple answers to this question based on the scenario. Below is one such answer.

#### ✅ Use Case: Ranking Users Based on Activity
Imagine you're working with a table user_actions that logs every action taken by users. You want to find the top 3 most active users per month based on the number of actions.

📊 Problem:

You need to:
* Count actions per user per month
* Rank them
* Filter only the top 3 per month

```sql
WITH ranked_users AS (
    SELECT
        user_id,
        DATE_TRUNC('month', action_date) AS action_month,
        COUNT(*) AS total_actions,
        RANK() OVER (PARTITION BY DATE_TRUNC('month', action_date) ORDER BY COUNT(*) DESC) AS user_rank
    FROM user_actions
    GROUP BY user_id, DATE_TRUNC('month', action_date)
)
SELECT *
FROM ranked_users
WHERE user_rank <= 3;
```

---

### 62. How often you use sql in day to day life?
These are common interview questions, and the answers may vary based on roles and responsibilities. You can manage the responses using the information below.

I use SQL on a daily basis as it's essential for data retrieval, analysis, and reporting. Whether it's pulling metrics, creating dashboards, validating datasets, or preparing inputs for machine learning models, SQL is the first step in my data workflow. I often write queries involving joins, aggregations, window functions, and CTEs to break down complex problems into manageable steps.

🧠 You can also customize your answer depending on your role:
* Data Analyst:
"I use SQL every day to query large datasets, generate reports, and explore data trends. It’s my primary tool for building insights before visualizing them in BI tools."
* Data Engineer:
"I use SQL daily to validate pipeline outputs, monitor data quality, and manage data transformations in ETL processes."
---

### 63. Differences between cte and view
| Feature          | CTE (Common Table Expression)                            | View                                              |
| ---------------- | -------------------------------------------------------- | ------------------------------------------------- |
| **Definition**   | Temporary, inline named query within a SQL statement     | Named, saved query stored in the database catalog |
| **Scope**        | Only visible to the query it’s defined in                | Globally accessible across queries/users          |
| **Persistence**  | Exists only during query execution                       | Persists in the database until explicitly dropped |
| **Performance**  | Recomputed every time the query runs (unless optimized)  | Can be materialized (depending on system support) |
| **Use Case**     | Useful for breaking down complex logic in a single query | Reusable logic shared across multiple queries     |
| **Syntax**       | `WITH cte_name AS (...)`                                 | `CREATE VIEW view_name AS ...`                    |
| **Modification** | Cannot be directly queried or updated outside its query  | Can sometimes be updatable (if simple enough)     |

🧠 When to Use What?
#### ✅ Use CTE when:
  * You need temporary logical structuring
  * Writing a one-time or complex query
  * Avoiding clutter with nested subqueries

#### ✅ Use View when:
  * You need reusability across teams
  * Want to abstract away complex logic
  * Need to apply consistent business logic in multiple places
---

### 64. Difference types of relationships in sql
In SQL, relationships between tables define how data in one table is related to data in another table. There are **four primary types of relationships** in relational databases: **one-to-one**, **one-to-many**, **many-to-one**, and **many-to-many**. Here's a detailed explanation:


## **Types of Relationships in SQL**

### 1. **One-to-One Relationship**

- **Definition**: In a one-to-one relationship, each record in the first table is related to **only one** record in the second table, and vice versa.
- **Use Case**: This is often used for splitting data into separate tables for logical or security purposes, or when dealing with very large data that should be split for performance.
- **Example**: A `person` table and a `passport` table where each person has one passport, and each passport belongs to only one person.

#### Example SQL:
```sql
CREATE TABLE person (
    person_id INT PRIMARY KEY,
    name VARCHAR(100)
);

CREATE TABLE passport (
    passport_id INT PRIMARY KEY,
    person_id INT UNIQUE,  -- One-to-One relationship
    passport_number VARCHAR(50),
    FOREIGN KEY (person_id) REFERENCES person(person_id)
);
```

### 2. **One-to-Many Relationship**

- **Definition**: In a one-to-many relationship, a single record in the first table can be related to **multiple records** in the second table, but each record in the second table can only be related to **one** record in the first table.
- **Use Case**: This is the most common relationship in databases. For example, one `customer` can have many `orders`.
- **Example**: A `department` table and an `employee` table where one department can have many employees, but each employee belongs to one department.

#### Example SQL:
```sql
CREATE TABLE department (
    department_id INT PRIMARY KEY,
    department_name VARCHAR(100)
);

CREATE TABLE employee (
    employee_id INT PRIMARY KEY,
    employee_name VARCHAR(100),
    department_id INT,
    FOREIGN KEY (department_id) REFERENCES department(department_id)
);
```

### 3. **Many-to-One Relationship**

- **Definition**: A many-to-one relationship is essentially the reverse of the one-to-many relationship. In this relationship, multiple records in the first table can be related to **one record** in the second table.
- **Use Case**: This relationship is used when many entities reference the same entity. For example, multiple `orders` can belong to a single `customer`.
- **Example**: A `product` table and a `category` table where many products belong to one category.

#### Example SQL:
```sql
CREATE TABLE category (
    category_id INT PRIMARY KEY,
    category_name VARCHAR(100)
);

CREATE TABLE product (
    product_id INT PRIMARY KEY,
    product_name VARCHAR(100),
    category_id INT,
    FOREIGN KEY (category_id) REFERENCES category(category_id)
);
```

### 4. **Many-to-Many Relationship**

- **Definition**: A many-to-many relationship occurs when multiple records in the first table can be related to **multiple records** in the second table, and vice versa. This relationship typically requires an **intersection table** (also known as a junction or linking table) to manage the associations between the two tables.
- **Use Case**: This is used when entities need to be related in multiple ways. For example, a `student` can enroll in many `courses`, and a `course` can have many `students`.
- **Example**: A `student` table, a `course` table, and a `student_course` table that links students to their enrolled courses.

#### Example SQL:
```sql
CREATE TABLE student (
    student_id INT PRIMARY KEY,
    student_name VARCHAR(100)
);

CREATE TABLE course (
    course_id INT PRIMARY KEY,
    course_name VARCHAR(100)
);

CREATE TABLE student_course (
    student_id INT,
    course_id INT,
    PRIMARY KEY (student_id, course_id),
    FOREIGN KEY (student_id) REFERENCES student(student_id),
    FOREIGN KEY (course_id) REFERENCES course(course_id)
);
```

## **Summary Table**

| Relationship Type   | Definition                                                                 | Example                                                                                           |
|---------------------|---------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| **One-to-One**       | Each record in Table A relates to one record in Table B and vice versa.   | A `person` has one `passport`.                                                                   |
| **One-to-Many**      | A record in Table A can relate to many records in Table B.                | A `department` has many `employees`.                                                              |
| **Many-to-One**      | Many records in Table A relate to one record in Table B.                 | Many `orders` are placed by one `customer`.                                                       |
| **Many-to-Many**     | Many records in Table A relate to many records in Table B (requires a junction table). | Many `students` enroll in many `courses`.                                                          |

## **When to Use Each Relationship**

- **One-to-One**: Use this when you want to break up data for performance or security reasons (e.g., personal information and sensitive data).
- **One-to-Many**: Most common in transactional systems (e.g., one customer placing many orders).
- **Many-to-One**: When many entities refer to a single entity (e.g., multiple employees in a single department).
- **Many-to-Many**: Use when both entities have multiple relationships with each other (e.g., students enrolling in multiple courses).
---
### 65. Desktop-Only Users:
Write a query that returns the company with the highest number of users that use desktop only.

#### 🧠 Assumptions:

There is a users table with at least the following columns:
* user_id
* customer_id
* device_type (e.g., 'desktop', 'mobile', 'tablet')

```sql
SELECT company_id
FROM users
WHERE user_id IN (
    SELECT user_id
    FROM users
    GROUP BY user_id
    HAVING COUNT(DISTINCT device_type) = 1
       AND MAX(device_type) = 'desktop'
)
GROUP BY company_id
ORDER BY COUNT(*) DESC
LIMIT 1;
```
#### Explanation:
* Identify users who use only one type of device and that device is 'desktop'.
* Group those users by company_id and count them.
* Return the company_id with the highest number of such users.
---

### 66. Most Popular Client ID
Select the most popular client_id based on the number of users who have at least 50% of their events from the following list:

* video call received
* video call sent
* voice call received
* voice call sent

#### 🧠 Assumptions:

There is an events table with at least the following columns:
* user_id
* client_id
* event_type

```sql
WITH user_event_stats AS (
    SELECT
        user_id,
        client_id,
        COUNT(*) AS total_events,
        SUM(CASE WHEN event_type IN (
            'video call received', 'video call sent',
            'voice call received', 'voice call sent'
        ) THEN 1 ELSE 0 END) AS call_events
    FROM events
    GROUP BY user_id, client_id
),
qualified_users AS (
    SELECT client_id
    FROM user_event_stats
    WHERE call_events * 1.0 / total_events >= 0.5
)
SELECT client_id
FROM qualified_users
GROUP BY client_id
ORDER BY COUNT(*) DESC
LIMIT 1;
```
---

### 67. Bottom Companies by Mobile Usage
Write a query that returns a list of the bottom 2 companies by mobile usage. 
* Company is defined in the customer_id column.
* Mobile usage is defined as the number of events registered on a client_id == 'mobile'.
* Order the result by the number of events ascending.
* In the case where there are multiple companies tied for the bottom ranks (rank 1 or 2), return all the companies.
* Output the customer_id and number of events.

#### 🧠 Assumptions:

There is an events table with at least the following columns:
customer_id
client_id

```sql
WITH mobile_events AS (
    SELECT customer_id, COUNT(*) AS mobile_event_count
    FROM events
    WHERE client_id = 'mobile'
    GROUP BY customer_id
),
ranked_companies AS (
    SELECT customer_id, mobile_event_count,
           DENSE_RANK() OVER (ORDER BY mobile_event_count ASC) AS rank
    FROM mobile_events
)
SELECT customer_id, mobile_event_count
FROM ranked_companies
WHERE rank <= 2
ORDER BY mobile_event_count ASC;
```
---

### 68. Exclusive Users per Client
Write a query that returns the number of users who are exclusive to only one client. Output the client_id and the number of such exclusive users.
#### 🧠 Assumptions:

There is an events table with at least the following columns:
* user_id
* client_id

```sql
WITH user_clients AS (
    SELECT user_id, client_id
    FROM events
    GROUP BY user_id, client_id
),
exclusive_users AS (
    SELECT user_id
    FROM user_clients
    GROUP BY user_id
    HAVING COUNT(DISTINCT client_id) = 1
),
exclusive_user_clients AS (
    SELECT uc.client_id
    FROM user_clients uc
    JOIN exclusive_users eu ON uc.user_id = eu.user_id
)
SELECT client_id, COUNT(*) AS exclusive_user_count
FROM exclusive_user_clients
GROUP BY client_id;
```
#### 💡 Explanation:
* Identify users who are associated with only one client_id.
* Count how many such users exist per client_id.

---

### 69. Unique Users per Client per Month
Write a query that returns the number of unique users per client_id per month.
#### 🧠 Assumptions:

There is an events table with at least the following columns:
* user_id
* client_id
* event_time (a timestamp or date column)
  
```sql
SELECT
    client_id,
    DATE_TRUNC('month', event_time) AS month,
    COUNT(DISTINCT user_id) AS unique_users
FROM events
GROUP BY client_id, DATE_TRUNC('month', event_time)
ORDER BY month, client_id;
```
#### 💡 Explanation:

* Use DATE_TRUNC('month', event_time) to group events by month.
* Count distinct user_ids per client_id per month.
* Order results chronologically and by client.
---

### 70. How would you optimize a slow-running query with multiple joins?

Optimizing slow queries with multiple joins involves several strategies:

1.  **Analyze the Execution Plan:** Use `EXPLAIN` (or its equivalent in your database system) to understand how the database is executing the query. This will highlight potential bottlenecks like full table scans or inefficient join algorithms.

2.  **Ensure Proper Indexing:** Verify that the columns involved in the `JOIN` conditions and `WHERE` clauses are properly indexed. The database can then use these indexes to quickly locate matching rows instead of scanning entire tables. Consider composite indexes for columns frequently used together.

3.  **Rewrite the Query:** Sometimes, the structure of the query itself can be inefficient. Consider:
    * **Joining on the correct columns:** Ensure you are joining on the most selective and appropriate keys.
    * **Filtering early:** Apply `WHERE` clause conditions as early as possible in the query to reduce the number of rows that need to be joined.
    * **Avoiding unnecessary joins:** Only join tables that are absolutely necessary to retrieve the required data.
    * **Using appropriate join types:** Understand the differences between `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, and `FULL OUTER JOIN` and use the most suitable type for your needs. Incorrect join types can lead to unexpected performance issues.

4.  **Optimize Data Types:** Ensure that the data types of the join columns are compatible. Implicit data type conversions can hinder index usage and slow down the query.

5.  **Consider Database Statistics:** Ensure your database has up-to-date statistics on the data distribution. The query optimizer uses these statistics to make informed decisions about the execution plan. Regularly update statistics, especially after significant data changes.

6.  **Partitioning (for large tables):** If the tables involved are very large, consider partitioning them based on a relevant column. This can significantly reduce the amount of data the database needs to scan during joins.

7.  **Denormalization (use with caution):** In some cases, and with careful consideration of data integrity implications, denormalizing the database schema by adding redundant columns to tables can reduce the need for complex joins.

8.  **Limit Results:** If you don't need all the rows, use `LIMIT` to reduce the amount of data processed and returned.
By systematically investigating these areas, you can often identify and resolve the performance bottlenecks in your SQL queries with multiple joins.
---
### 71. What is a Recursive CTE, and when would you use it?

A **Recursive Common Table Expression (CTE)** is a powerful SQL construct that allows you to define a CTE that refers to itself. This enables you to query hierarchical or recursive data structures, such as organizational charts, bill-of-materials, or graph traversals.

A recursive CTE typically consists of two parts:

1.  **Anchor Member:** This is the base case of the recursion. It's a non-recursive query that returns the initial set of rows.

2.  **Recursive Member:** This part is a query that refers to the CTE itself (the "recursive" part). It operates on the results of the previous iteration and generates the subsequent set of rows.

The process continues iteratively until the recursive member returns no more rows. The final result is the union of all the result sets from each iteration.

**Example of When to Use It:**

Consider an **organizational hierarchy** represented in a table called `Employees` with columns `EmployeeID`, `EmployeeName`, and `ManagerID`. You want to retrieve a list of all subordinates for a given employee. A recursive CTE is ideal for this:

```sql
WITH RECURSIVE Subordinates AS (
    -- Anchor member: Select the initial employee
    SELECT EmployeeID, EmployeeName, ManagerID
    FROM Employees
    WHERE EmployeeID = 101 -- Replace with the ID of the top-level employee

    UNION ALL

    -- Recursive member: Find subordinates of the employees selected in the previous iteration
    SELECT e.EmployeeID, e.EmployeeName, e.ManagerID
    FROM Employees e
    INNER JOIN Subordinates s ON e.ManagerID = s.EmployeeID
)
SELECT EmployeeID, EmployeeName
FROM Subordinates
WHERE EmployeeID <> 101; -- Exclude the top-level employee from the final result
```
#### 💡 Explanation of the Example:

* The anchor member selects the row for the employee with EmployeeID = 101 (the top of the hierarchy we're starting from).
* The recursive member then joins the Employees table (e) with the Subordinates CTE (s) on the condition that the employee's ManagerID matches the EmployeeID of someone already in the Subordinates CTE (from the previous iteration). This effectively finds the direct reports of the previously selected employees.
* The UNION ALL combines the results of the anchor and recursive members.
* The recursion continues until no more employees have a ManagerID that matches an EmployeeID in the Subordinates CTE.
---
### 72. Explain the difference between clustered and non-clustered indexes and when to use each.

In SQL, indexes are used to speed up data retrieval operations. There are two main types of indexes: clustered and non-clustered.

**Clustered Index:**

* A clustered index determines the **physical order** of the data in a table. Think of it like a dictionary where the words are physically arranged in alphabetical order.
* A table can have **only one** clustered index because the data can only be physically sorted in one way.
* Typically, the primary key of a table is used to define the clustered index, although you can choose a different column.
* The leaf nodes of a clustered index **contain the actual data rows** of the table.

**Non-Clustered Index:**

* A non-clustered index is a separate structure from the data rows. It contains a **copy of the indexed columns** and a **pointer** to the actual data row in the table (which is located by the clustered index if one exists, or by the physical row identifier if the table is a heap - has no clustered index).
* A table can have **multiple** non-clustered indexes. Think of it like the index at the back of a book; it lists keywords and the page numbers where they can be found.
* The leaf nodes of a non-clustered index contain the indexed key values and a row locator (either the clustered key or a RowID).

**When to Use Each:**

**Clustered Index:**

* **Columns frequently used in range queries or sorting:** Since the data is physically ordered, retrieving a range of values or sorting by the clustered index column is very efficient.
* **Columns that are unique and non-null:** Primary keys are excellent candidates for clustered indexes as they enforce uniqueness and provide an efficient way to identify each row.
* **Tables where you often retrieve entire rows:** Because the leaf nodes contain the actual data, retrieving all columns for a set of rows based on the clustered index is fast.

**Consider NOT using a clustered index on:**

* **Columns that are frequently updated:** Updates to the clustered index column can be expensive as it requires physically reordering the data rows.
* **Columns with many non-unique values:** While allowed, it can lead to extra overhead as the database needs to add a uniqueifier to each non-unique key value.

**Non-Clustered Index:**

* **Columns frequently used in `WHERE` clauses:** Non-clustered indexes can significantly speed up queries that filter data based on specific column values.
* **Columns involved in `JOIN` conditions:** Creating non-clustered indexes on join columns in multiple tables can improve the performance of join operations.
* **Columns used in `SELECT` statements along with the filtering columns:** If a query frequently selects a small set of columns that are also used in the `WHERE` clause, a covering non-clustered index (an index that includes all the columns needed by the query) can be very efficient as the database can retrieve all the necessary data directly from the index without accessing the base table.
* **Columns with high cardinality (many unique values):** Non-clustered indexes are generally more effective on columns with a large number of distinct values.

**In Summary:**

| Feature          | Clustered Index                     | Non-Clustered Index                         |
| ---------------- | ----------------------------------- | ------------------------------------------- |
| Physical Order   | Yes                                 | No                                          |
| Number per Table | One                                 | Multiple                                    |
| Leaf Node        | Contains the actual data rows       | Contains indexed columns and a row locator |
| Best For         | Range queries, sorting, unique IDs, retrieving entire rows | Filtering, joins, covering queries        |
---
### 73. SQL Query to Find the Second Highest Salary in Each Department

**Assumptions:**

* `Employees` table contains:
    * `EmployeeID` (INT, Primary Key)
    * `EmployeeName` (VARCHAR)
    * `DepartmentID` (INT, Foreign Key to `Departments`)
    * `Salary` (DECIMAL or INT)
* `Departments` table contains:
    * `DepartmentID` (INT, Primary Key)
    * `DepartmentName` (VARCHAR)

**Query:**

```sql
WITH RankedSalaries AS (
    SELECT
        e.EmployeeID,
        e.DepartmentID,
        e.EmployeeName,
        d.DepartmentName,
        e.Salary,
        DENSE_RANK() OVER (PARTITION BY e.DepartmentID ORDER BY e.Salary DESC) as SalaryRank
    FROM
        Employees e
    JOIN
        Departments d ON e.DepartmentID = d.DepartmentID
)
SELECT
    EmployeeName,
    DepartmentName,
    Salary AS SecondHighestSalary
FROM
    RankedSalaries
WHERE
    SalaryRank = 2;
```
---
### 74. How would you detect and resolve deadlocks in SQL?

Deadlocks occur when two or more transactions are blocked indefinitely because each transaction holds a lock that the other transaction needs. Detecting and resolving them is crucial for maintaining database performance and availability.

**Detection:**

1.  **Monitoring System Logs:** Most database systems log information about deadlocks. Regularly reviewing these logs can help identify if deadlocks are occurring. Look for specific error messages or events indicating a deadlock situation.

2.  **Performance Monitoring Tools:** Many database performance monitoring tools can detect and alert you to deadlocks in real-time. These tools often provide insights into the transactions and resources involved.

3.  **System Views and DMVs (Dynamic Management Views):** SQL Server and other database systems provide system views or DMVs that expose information about active locks, blocked processes, and deadlock graphs. Querying these views can help in identifying current deadlocks and their causes.

    * **SQL Server:**
        * `sys.dm_os_waiting_tasks`: Shows tasks that are currently waiting for a resource.
        * `sys.dm_tran_locks`: Provides information about active lock requests.
        * `sys.dm_tran_session_transactions`: Shows information about the current transactions for each session.
        * `sys.dm_os_threads`: Can sometimes provide context about the threads involved in deadlocks.
        * `sys.dm_os_schedulers`: Information about the SQL Server scheduler.
        * **Deadlock Graph (Extended Events or Trace Flags):** Configuring Extended Events or enabling trace flag 1204 or 1222 in SQL Server can capture detailed information about the deadlock, including the processes, resources, and the order of lock requests. This is invaluable for root cause analysis.

    * **PostgreSQL:**
        * `pg_locks`: Provides information about the locks held by database objects.
        * `pg_stat_activity`: Shows information about the currently executing queries.

    * **MySQL:**
        * `SHOW ENGINE INNODB STATUS`: Provides detailed information about the InnoDB storage engine, including recent deadlocks.
        * Performance Schema tables like `events_waits_current` and `data_locks`.

4.  **Application-Level Monitoring:** Sometimes, application behavior like long-running transactions or frequent contention on specific resources can be indicators of potential deadlocks.

**Resolution:**

Most database systems have a built-in **deadlock detection mechanism**. When a deadlock is detected, the database engine will choose one of the involved transactions as the **victim** and roll it back, releasing its locks so that the other transaction(s) can proceed. The application receiving the rollback error (e.g., "deadlock victim") should be designed to **retry the transaction automatically** after a short delay.

Beyond the automatic resolution, here are strategies to **prevent or minimize** deadlocks:

1.  **Keep Transactions Short and Fast:** Shorter transactions hold locks for a shorter duration, reducing the window for deadlocks to occur.

2.  **Access Resources in the Same Order:** If multiple transactions consistently access the same tables or rows in the same order, it reduces the chance of a circular dependency of locks. Implement a consistent order of operations within your application logic.

3.  **Use Appropriate Isolation Levels:** Higher isolation levels (like Serializable) reduce the likelihood of concurrency issues but can increase the chance of deadlocks. Choose the lowest isolation level that still ensures data consistency for your application.

4.  **Minimize Lock Duration:** Avoid holding locks for longer than necessary. Commit or rollback transactions as soon as the work is complete.

5.  **Avoid User Interaction within Transactions:** If a transaction involves waiting for user input, the locks held by that transaction can block other transactions for an extended period, increasing the risk of deadlocks.

6.  **Use Optimistic Locking:** Instead of exclusive locks, optimistic locking involves checking if the data has changed since it was last read before applying an update. If it has changed, the update fails, and the transaction can be retried. This reduces the need for explicit locking.

7.  **Consider Using Lower Isolation Levels:** While ensuring data integrity is paramount, sometimes using a slightly lower isolation level (if appropriate for the application's needs) can reduce locking and the potential for deadlocks.

8.  **Optimize Queries:** Slow-running queries can hold locks for longer periods. Optimize your queries by adding appropriate indexes, rewriting inefficient queries, etc.

9.  **Partitioning Data:** For very large tables, partitioning can reduce contention by dividing the data into smaller, more manageable units.

10. **Careful Indexing:** While indexes generally improve performance, excessive or poorly chosen indexes can sometimes lead to increased locking and potential deadlocks, especially during write operations.

By proactively implementing these strategies and diligently monitoring your database system, you can significantly reduce the occurrence and impact of deadlocks. When deadlocks do occur, understanding how to detect them and ensuring your application can gracefully handle rollback errors and retry transactions are essential for a robust and reliable system.

---
### 75. Write a query to find the top-performing ads based on click-through rate.

```sql
SELECT
    ad_id,
    (clicks / impressions) * 100 AS ctr
FROM
    ads
WHERE impressions > 0 -- Avoid division by zero
ORDER BY
    ctr DESC
LIMIT ; 
```
---
### 76. Identifying Active Users in User Login Logs

To identify active users from a dataset of user login logs, you'll typically look for users who have logged in within a specific recent timeframe. The definition of "active" can vary depending on your application and its usage patterns. Here's a general approach and a sample SQL query to illustrate:

**General Approach:**

1.  **Identify the Relevant Data:** You need a table or data structure that stores user login events. This should ideally include:
    * A unique user identifier (e.g., `UserID`).
    * A timestamp of the login event (e.g., `LoginTimestamp`).

2.  **Define the "Active" Timeframe:** Determine the period within which a login qualifies a user as "active". This could be:
    * The last day
    * The last week
    * The last month
    * A custom rolling window (e.g., any login in the past 30 days)

3.  **Query the Data:** Construct a query to filter the login logs and find users with login events within the defined timeframe.

4.  **Extract Unique Users:** Once you have the relevant login records, extract the unique user identifiers to get a list of active users.

**Sample SQL Query (assuming a table named `LoginLogs`):**

Let's assume you want to identify users who have logged in within the last 30 days.

```sql
SELECT DISTINCT
    UserID
FROM
    LoginLogs
WHERE
    LoginTimestamp >= date('now', '-30 days');
```
---

### 77. Given a table of user activity logs, write a query to calculate the daily active users (DAU).

```sql
SELECT
    DATE(activity_time) AS activity_date,
    COUNT(DISTINCT user_id) AS daily_active_users
FROM
    user_activity
GROUP BY
    activity_date
ORDER BY
    activity_date;
```
---

### 78. Write a query to segment users based on their engagement levels.
If we dont have any information, we can take below assumption and answer the query.

#### 🧠 Assumptions:
* We have a table named user_activity with the following columns:
  * user_id (unique identifier for each user)
  * last_login_date (date of the user's last login)
  * total_sessions (total number of sessions in the last 30 days)
  * avg_session_duration (average session duration in minutes)
  * content_interactions (number of content interactions like likes, comments, shares)

#### Engagement Segmentation Criteria:
Lets define three levels of engagement:

* **Highly Engaged**:
  * total_sessions >= 15
  * avg_session_duration >= 10
  * content_interactions >= 20
* **Moderately Engaged**:
  * total_sessions BETWEEN 5 AND 14
  * avg_session_duration BETWEEN 5 AND 9.9
  * content_interactions BETWEEN 5 AND 19
* **Low Engagement**:
  * Anything below the thresholds for Moderate Engagement
 
```sql
SELECT 
    user_id,
    CASE 
        WHEN total_sessions >= 15 
             AND avg_session_duration >= 10 
             AND content_interactions >= 20 THEN 'Highly Engaged'
        WHEN total_sessions BETWEEN 5 AND 14 
             AND avg_session_duration BETWEEN 5 AND 9.9 
             AND content_interactions BETWEEN 5 AND 19 THEN 'Moderately Engaged'
        ELSE 'Low Engagement'
    END AS engagement_level
FROM user_activity;
```

---

### 79. Average Post Hiatus
Average Post Hiatus typically refers to the average length of time between a user's posts on a specific platform or across multiple platforms. It measures the typical gaps or breaks in someone's posting activity.

#### 🧠 Assumptions:
Facebook_posts with the following columns:
* user_id – ID of the user who made the post
* post_date – Date of the post (in DATE format)

```sql
SELECT 
    user_id,
    DATEDIFF(MAX(post_date), MIN(post_date)) AS days_between_first_and_last_post
FROM 
    facebook_posts
WHERE 
    YEAR(post_date) = 2024
GROUP BY 
    user_id
HAVING 
    COUNT(*) >= 2;
```
---

### 80. Facebook Power Users
A Facebook power user is defined as someone who posts a ton and gets a lot of reactions on their post. For the purpose of this question, consider a Facebook power user as someone who posts at least twice a day and receives an average of 150 comments and/or reactions per post. Write a SQL query to return the IDs of all Facebook power users, along with the number of posts, and the average number of reactions per post.

* user_post table: user_id (integer), post_id (integer), post_date (timestamp)
* post_interactions table: post_id (integer), comments (integer), reactions (integer)

To identify Facebook power users, we need to:

* Calculate the number of posts per user per day.
* Filter users who post at least twice a day on average.
* Calculate the average number of comments and reactions per post.
* Filter users with an average of at least 150 interactions per post.

```sql
WITH daily_post_counts AS (
    SELECT 
        user_id,
        DATE(post_date) AS post_day,
        COUNT(*) AS posts_per_day
    FROM user_post
    GROUP BY user_id, DATE(post_date)
),
users_with_high_post_frequency AS (
    SELECT 
        user_id
    FROM daily_post_counts
    GROUP BY user_id
    HAVING AVG(posts_per_day) >= 2
),
post_interaction_totals AS (
    SELECT 
        up.user_id,
        COUNT(up.post_id) AS total_posts,
        SUM(pi.comments + pi.reactions) * 1.0 / COUNT(up.post_id) AS avg_interactions_per_post
    FROM user_post up
    JOIN post_interactions pi ON up.post_id = pi.post_id
    GROUP BY up.user_id
),
power_users AS (
    SELECT 
        pit.user_id,
        pit.total_posts,
        pit.avg_interactions_per_post
    FROM post_interaction_totals pit
    JOIN users_with_high_post_frequency uwhpf ON pit.user_id = uwhpf.user_id
    WHERE pit.avg_interactions_per_post >= 150
)

SELECT * FROM power_users;
```
---

### 81. Active User Retention
Assume you’re given a table containing information on Facebook user actions. Write a SQL query to obtain the number of monthly active users (MAUs) in July 2022, including the month in numerical format “1, 2, 3”. Hint: An active user is defined as a user who has performed actions such as ‘sign-in’, ‘like’, or ‘comment’ in both the current month and the previous month.

* user_actions table: user_id (integer), event_id (integer), event_type (string), event_date (datetime)

```sql
WITH filtered_actions AS (
    SELECT 
        user_id,
        EXTRACT(MONTH FROM event_date) AS month,
        EXTRACT(YEAR FROM event_date) AS year
    FROM user_actions
    WHERE event_type IN ('sign-in', 'like', 'comment')
      AND event_date BETWEEN '2022-06-01' AND '2022-07-31'
),
monthly_users AS (
    SELECT DISTINCT user_id, month
    FROM filtered_actions
    WHERE year = 2022
)

SELECT 
    7 AS month,
    COUNT(DISTINCT ju.user_id) AS monthly_active_users
FROM 
    monthly_users ju
JOIN 
    monthly_users ju_prev
    ON ju.user_id = ju_prev.user_id
WHERE 
    ju.month = 7 AND ju_prev.month = 6;
```

### 82. Facebook Friend Recommendations
Facebook wants to recommend new friends to people who show interest in attending 2 or more of the same private Facebook events. Write a SQL query to find pairs of friends to be recommended to each other if they’re interested in attending 2 or more of the same private events.

**Notes**:
* A user interested in attending would have either ‘going’ or ‘maybe’ as their attendance status.
* Friend recommendations are unidirectional, meaning if user x and user y should be recommended to each other, the result table should have both user x recommended to user y and user y recommended to user x.
* The result should not contain duplicates (i.e., user y should not be recommended to user x multiple times).

**schema**:
* friendship_status table: user_a_id (integer), user_b_id (integer), status (enum: ‘friends’, ‘not_friends’)
* event_rsvp table: user_id (integer), event_id (integer), event_type (enum: ‘public’, ‘private’), attendance_status (enum: ‘going’, ‘maybe’, ‘not_going’), event_date (date)

To find pairs of users who should be recommended to each other based on shared interest in 2 or more of the same private events.
1. Filters for users who RSVP'd as 'going' or 'maybe' to private events.
2. Finds user pairs who have RSVP'd to the same private events.
3. Counts the number of shared events per user pair.
4. Filters for pairs with 2 or more shared events.
5. Ensures the users are not already friends.
6. Outputs both directions of the recommendation (i.e., x → y and y → x).
7. Avoids duplicate recommendations.

```sql
WITH interested_users AS (
    SELECT user_id, event_id
    FROM event_rsvp
    WHERE event_type = 'private'
      AND attendance_status IN ('going', 'maybe')
),
shared_events AS (
    SELECT iu1.user_id AS user_a, iu2.user_id AS user_b, COUNT(*) AS shared_event_count
    FROM interested_users iu1
    JOIN interested_users iu2
      ON iu1.event_id = iu2.event_id
     AND iu1.user_id < iu2.user_id
    GROUP BY iu1.user_id, iu2.user_id
    HAVING COUNT(*) >= 2
),
non_friends AS (
    SELECT se.user_a, se.user_b
    FROM shared_events se
    LEFT JOIN friendship_status fs
      ON (se.user_a = fs.user_a_id AND se.user_b = fs.user_b_id)
         OR (se.user_a = fs.user_b_id AND se.user_b = fs.user_a_id)
    WHERE fs.status IS NULL OR fs.status != 'friends'
)
SELECT user_a AS recommender, user_b AS recommended
FROM non_friends
UNION
SELECT user_b AS recommender, user_a AS recommended
FROM non_friends;
```
**🗣️ Explanation**:
* interested_users: Filters only those users who are interested in private events.
* shared_events: Finds unique user pairs who share the same private events and counts them.
* non_friends: Filters out pairs who are already friends.
* Final SELECT with UNION: Ensures both directions of recommendation are included without duplicates.
---
### 83. What is Cardinality
Cardinality in databases refers to the uniqueness and relationships of data values within tables. It plays a crucial role in database design, indexing, and query optimization.

#### 🔹 1. Column Cardinality
Column cardinality describes the number of distinct values in a column.
* High Cardinality: Many unique values
    * Example: Email addresses, UUIDs, phone numbers.
* Low Cardinality: Few unique values
    * Example: Boolean flags, gender, status fields.
* Medium Cardinality: Moderate number of unique values
    * Example: U.S. states, product categories.

Understanding column cardinality helps the database engine choose efficient indexes and query plans.

#### 2. Relationship Cardinality
Relationship cardinality defines how tables relate to each other:

* One-to-One (1:1)
Each row in Table A relates to exactly one row in Table B.
* One-to-Many (1:N)
A row in Table A can relate to multiple rows in Table B.
* Many-to-Many (M:N)
Multiple rows in Table A can relate to multiple rows in Table B.

Implemented using a junction (bridge) table.

#### Why Cardinality Matters
* Helps in database normalization.
* Influences indexing strategies.
* Improves query performance.
* Aids in creating efficient and scalable data models.
---
### 84. ⁠How do you calculate the median of a numeric column in SQL?

Standard approach using subqueries
```sql
SELECT AVG(val) AS median
FROM (
    SELECT val
    FROM your_table
    WHERE val IS NOT NULL
    ORDER BY val
    LIMIT 2 - (SELECT COUNT(*) FROM your_table WHERE val IS NOT NULL) % 2  -- 1 if odd, 2 if even
    OFFSET (SELECT (COUNT(*) - 1) / 2 FROM your_table WHERE val IS NOT NULL)
) AS median_values;
```

#### Explanation
* Ensures only valid numeric values are considered.
* Used multiple times to determine how many values are in the column.
* Median requires values to be sorted.
* Calculate how many values to take
    * If the count is odd, LIMIT = 1 (get the middle value).
    * If the count is even, LIMIT = 2 (get the two middle values).
* Calculate where to start (offset)
    * The middle value (if odd count),
    * The first of the two middle values (if even count).
---
### 85 Write a query to find duplicate rows in a dataset.

Assuming the employee table.
```sql
SELECT emp_name, emp_id, -- Add all columns that define a "row"
       COUNT(*) AS duplicate_count
FROM emp
GROUP BY emp_name, emp_id -- Group by the same columns
HAVING COUNT(*) > 1;
```
---
### 86. Write a query to calculate the rolling average of sales for the past 7 days.
To analyze trends over time, we can use rolling average of data.
```sql
SELECT
    sales_date,
    SUM(sales_amount) AS daily_sales,
    AVG(SUM(sales_amount)) OVER (
        ORDER BY sales_date
        ROWS BETWEEN 6 PRECEDING AND CURRENT ROW
    ) AS rolling_avg_7_days
FROM sales_table
GROUP BY sales_date
ORDER BY sales_date;

```
---
### 87. Write a query to extract users who performed at least 5 transactions in a month.

This query retrieves users who have performed **at least 5 transactions in a single month**. It is useful for identifying high-engagement users or filtering for loyalty analysis.

### 🔍 SQL Query

```sql
SELECT user_id, 
       DATE_TRUNC('month', transaction_date) AS month,
       COUNT(*) AS transaction_count
FROM transactions
GROUP BY user_id, DATE_TRUNC('month', transaction_date)
HAVING COUNT(*) >= 5
ORDER BY user_id, month;
```
---
### 88. How would you detect anomalies or outliers in a dataset using SQL?
You can detect anomalies by calculating statistical measures (like the mean and standard deviation) and then filtering rows that deviate too far from the mean. For example, to find rows where a value is more than 3 standard deviations away from the mean as below
#### 1. 📉 Using Standard Deviation (Z-score method)
```sql
WITH stats AS (
    SELECT 
        AVG(value) AS avg_value, 
        STDDEV(value) AS std_dev
    FROM your_table
)
SELECT 
    t.*,
    (t.value - s.avg_value) / s.std_dev AS z_score
FROM your_table t
CROSS JOIN stats s
WHERE ABS((t.value - s.avg_value) / s.std_dev) > 3;
```
#### 2. 🟨 Using Percentile Thresholds (IQR method)
```sql
WITH percentiles AS (
    SELECT
        PERCENTILE_CONT(0.25) WITHIN GROUP (ORDER BY value) AS Q1,
        PERCENTILE_CONT(0.75) WITHIN GROUP (ORDER BY value) AS Q3
    FROM data_table
)
SELECT *
FROM data_table, percentiles
WHERE value < Q1 - 1.5 * (Q3 - Q1)
   OR value > Q3 + 1.5 * (Q3 - Q1);
```
---
### 89. Write a query to pivot a table and convert rows into columns.


Pivoting is the process of transforming **row-based data into columnar format** — useful for creating summary reports where values in one column become separate columns in the result set.

#### 🧾 Example Use Case

Suppose you have a table `sales_data`:

| user_id | month | sales_amount |
|---------|-------|--------------|
| 1       | Jan   | 100          |
| 1       | Feb   | 150          |
| 2       | Jan   | 200          |
| 2       | Feb   | 250          |

The goal is to **pivot the `month` values into columns** like:

| user_id | Jan_sales | Feb_sales |
|---------|-----------|-----------|
| 1       | 100       | 150       |
| 2       | 200       | 250       |

---

#### ✅ SQL Query Using `CASE WHEN` (Database-Agnostic)

```sql
SELECT
    user_id,
    SUM(CASE WHEN month = 'Jan' THEN sales_amount ELSE 0 END) AS Jan_sales,
    SUM(CASE WHEN month = 'Feb' THEN sales_amount ELSE 0 END) AS Feb_sales
FROM sales_data
GROUP BY user_id;
```

#### 🛠 SQL Server Version Using PIVOT
```sql
SELECT user_id, [Jan], [Feb]
FROM (
    SELECT user_id, month, sales_amount
    FROM sales_data
) AS source
PIVOT (
    SUM(sales_amount) FOR month IN ([Jan], [Feb])
) AS pivot_table;
```
---
### 90. How can you rank users based on their total purchase value in descending order?
#### ✅ SQL Query Using `RANK()` or `DENSE_RANK()`

```sql
SELECT
    user_id,
    SUM(purchase_amount) AS total_purchase,
    RANK() OVER (ORDER BY SUM(purchase_amount) DESC) AS purchase_rank
FROM sales
GROUP BY user_id
ORDER BY purchase_rank;
```
---
### 91. What is ACLOVERRIDE
