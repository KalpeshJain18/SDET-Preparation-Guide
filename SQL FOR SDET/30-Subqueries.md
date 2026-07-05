# 🚀 SQL FOR SDET → Subqueries ⭐

Subqueries are one of the MOST IMPORTANT SQL concepts for:
- Writing complex SQL queries
- Backend data validation
- Nested data retrieval
- Product company interview questions

Interviewers ask this in:
- SQL interview rounds
- Product company interviews
- Backend testing discussions
- SDET technical rounds

--------------------------------------------------

# 🎯 Topics Covered

1. What is a Subquery
2. Why Subqueries are Important
3. Types of Subqueries
4. Subquery Syntax
5. Subquery with WHERE Clause
6. Correlated vs Non-Correlated Subqueries
7. Subquery vs JOIN
8. Real-Time Testing Scenarios
9. Performance Considerations
10. Common Mistakes
11. Common Interview Questions

--------------------------------------------------

# 🧠 1. What is a Subquery

## What is it

A Subquery is a query written inside another SQL query.

---

## Key Components

- Nested query
- Inner query
- Outer query
- Returns data to the outer query

---

## How to Answer (Interview Style)

A subquery is a SQL query nested inside another query. The result of the inner query is used by the outer query.

---

## Practical Example

```sql
SELECT name
FROM employees
WHERE department_id =
(
    SELECT id
    FROM departments
    WHERE department_name = 'IT'
);
```

---

## Common Mistakes

- Returning multiple rows when using the = operator
- Incorrect nesting of queries
- Missing parentheses

---

## Expected Interview Questions

- What is a subquery?
- Why are subqueries used?
- Can subqueries be nested?

--------------------------------------------------

# 🧠 2. Why Subqueries are Important ⭐

## What is it

Subqueries simplify complex business logic by breaking it into smaller queries.

---

## Key Components

- Dynamic filtering
- Business logic
- Nested queries
- Data retrieval

---

## How to Answer (Interview Style)

Subqueries make complex SQL queries easier to understand and maintain by dividing the problem into smaller parts.

---

## Practical Example

```text
Find employees working in the highest-paid department.
```

---

## Common Mistakes

- Using JOIN where a simple subquery is sufficient
- Creating unnecessary nested queries

---

## Expected Interview Questions

- Why are subqueries important?
- Give a real-world example.

--------------------------------------------------

# 🧠 3. Types of Subqueries ⭐

## Types

- Single-row Subquery
- Multiple-row Subquery
- Multiple-column Subquery
- Correlated Subquery
- Non-Correlated Subquery

---

## How to Answer (Interview Style)

SQL supports different types of subqueries depending on the number of rows returned and whether they depend on the outer query.

---

## Practical Example

```text
Single-row → Returns one value

Multiple-row → Returns multiple values

Correlated → Depends on outer query

Non-Correlated → Independent query
```

---

## Common Mistakes

- Using the wrong comparison operator
- Choosing the wrong type of subquery

---

## Expected Interview Questions

- What are the different types of subqueries?
- Which operators work with multiple-row subqueries?

--------------------------------------------------

# 🧠 4. Subquery Syntax ⭐

## What is it

A standard structure for writing nested SQL queries.

---

## Key Components

- Outer query
- Inner query
- Parentheses

---

## How to Answer (Interview Style)

The inner query executes first, and its result is passed to the outer query.

---

## Practical Example

```sql
SELECT *
FROM employees
WHERE salary >
(
    SELECT AVG(salary)
    FROM employees
);
```

---

## Common Mistakes

- Missing parentheses
- Incorrect placement of the subquery

---

## Expected Interview Questions

- What is the syntax of a subquery?
- Which query executes first?

--------------------------------------------------

# 🧠 5. Subquery with WHERE Clause ⭐

## What is it

The most common use of subqueries.

---

## Key Components

- Dynamic filtering
- Nested conditions
- Data retrieval

---

## How to Answer (Interview Style)

Subqueries inside the WHERE clause dynamically filter records based on the result of another query.

---

## Practical Example

```sql
SELECT *
FROM orders
WHERE customer_id IN
(
    SELECT id
    FROM customers
    WHERE city = 'Bangalore'
);
```

---

## Common Mistakes

- Using = instead of IN for multiple rows
- Returning multiple rows unexpectedly

---

## Expected Interview Questions

- How do you use subqueries with WHERE?
- Difference between IN and =?

--------------------------------------------------

# 🧠 6. Correlated vs Non-Correlated Subqueries ⭐

## Difference

| Correlated Subquery | Non-Correlated Subquery |
|----------------------|-------------------------|
| Depends on outer query | Independent |
| Executes repeatedly | Executes once |
| Slower | Faster |
| Uses values from outer query | Does not use outer query values |

---

## How to Answer (Interview Style)

A correlated subquery depends on the outer query for execution, whereas a non-correlated subquery executes independently.

---

## Practical Example

```text
Correlated → Compare each employee's salary with their department average.

Non-Correlated → Find employees earning above the company average salary.
```

---

## Common Mistakes

- Confusing execution behavior
- Using correlated subqueries unnecessarily

---

## Expected Interview Questions

- Correlated vs Non-Correlated subqueries?
- Which one performs better?

--------------------------------------------------

# 🧠 7. Subquery vs JOIN ⭐

## Difference

| Subquery | JOIN |
|----------|------|
| Nested query | Combines tables |
| Easier for simple logic | Better for relational data |
| Can be slower | Usually more efficient |
| Good for filtering | Good for retrieving related data |

---

## How to Answer (Interview Style)

Subqueries are useful for filtering and nested logic, while JOINs are generally preferred for combining related tables efficiently.

---

## Practical Example

```text
Subquery → Find employees earning above average salary.

JOIN → Retrieve employee names with department names.
```

---

## Common Mistakes

- Using subqueries where JOINs perform better
- Choosing JOIN when a simple subquery is sufficient

---

## Expected Interview Questions

- Subquery vs JOIN?
- Which performs better?

--------------------------------------------------

# 🧠 8. Real-Time Testing Scenarios ⭐

## Banking Applications

```text
Find accounts with balances greater than the average balance.
```

---

## E-Commerce Applications

```text
Find products whose sales exceed the category average.
```

---

## User Management Systems

```text
Find users with the highest login count.
```

---

## Automation Testing

```text
Identify test cases whose execution time is greater than the average execution time.
```

--------------------------------------------------

# 🧠 9. Performance Considerations ⭐

## What is it

Complex subqueries can impact performance, especially correlated subqueries.

---

## Key Components

- Index usage
- Query optimization
- Correlated subqueries
- Execution cost

---

## How to Answer (Interview Style)

Use JOINs instead of correlated subqueries whenever possible for better performance on large datasets.

---

## Practical Example

```text
Replace correlated subqueries with JOINs for large production tables.
```

---

## Common Mistakes

- Overusing correlated subqueries
- Ignoring query execution plans
- Not using indexes

---

## Expected Interview Questions

- How do you optimize subqueries?
- JOIN vs Subquery performance?

--------------------------------------------------

# 🧠 10. Common Mistakes ⭐

- Missing parentheses
- Using = instead of IN for multiple rows
- Returning multiple rows unexpectedly
- Overusing correlated subqueries
- Ignoring query performance
- Using subqueries when JOINs are more efficient

--------------------------------------------------

# 🧠 11. Common Interview Questions ⭐

- What is a subquery?
- What are the different types of subqueries?
- Correlated vs Non-Correlated subqueries?
- Subquery vs JOIN?
- Which is faster: JOIN or Subquery?
- Difference between IN and EXISTS?
- Real-world use cases?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. Types of Subqueries ⭐
2. Subquery with WHERE ⭐
3. Correlated vs Non-Correlated Subqueries ⭐
4. Subquery vs JOIN ⭐
5. Query Performance Optimization ⭐
6. Real-Time Business Scenarios ⭐

--------------------------------------------------
