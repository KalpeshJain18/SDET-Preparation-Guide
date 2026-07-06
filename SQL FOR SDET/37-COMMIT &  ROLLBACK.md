# 🚀 SQL FOR SDET → COMMIT / ROLLBACK ⭐

COMMIT and ROLLBACK are two of the MOST IMPORTANT Transaction Control Language (TCL) commands in SQL for:
- Saving database changes permanently
- Undoing failed transactions
- Maintaining data consistency
- Backend validation and recovery

Interviewers ask this in:
- SQL interview rounds
- Product company interviews
- Backend testing discussions
- SDET technical rounds

--------------------------------------------------

# 🎯 Topics Covered

1. What is COMMIT
2. What is ROLLBACK
3. Why COMMIT and ROLLBACK are Important
4. COMMIT Syntax
5. ROLLBACK Syntax
6. COMMIT vs ROLLBACK
7. SAVEPOINT
8. Real-Time Testing Scenarios
9. Performance Considerations
10. Common Mistakes
11. Common Interview Questions

--------------------------------------------------

# 🧠 1. What is COMMIT

## What is it

COMMIT permanently saves all changes made during the current transaction.

Once a transaction is committed, the changes become permanent and cannot be undone using ROLLBACK.

---

## Key Components

- Saves changes permanently
- Ends the current transaction
- Makes data visible to other users
- Cannot be undone using ROLLBACK

---

## How to Answer (Interview Style)

COMMIT permanently saves all successful changes made during a transaction. After COMMIT executes, the transaction ends and the changes become permanent.

---

## Practical Example

```sql
BEGIN TRANSACTION;

UPDATE employees
SET salary = salary + 5000
WHERE employee_id = 101;

COMMIT;
```

---

## Common Mistakes

- Forgetting to execute COMMIT
- Assuming changes are automatically saved
- Trying to rollback after COMMIT

---

## Expected Interview Questions

- What is COMMIT?
- When should COMMIT be used?
- Can COMMIT be undone?

--------------------------------------------------

# 🧠 2. What is ROLLBACK

## What is it

ROLLBACK cancels all changes made during the current transaction before they are committed.

It restores the database to the state before the transaction started.

---

## Key Components

- Cancels uncommitted changes
- Restores previous state
- Used during errors
- Ends the transaction

---

## How to Answer (Interview Style)

ROLLBACK reverses all changes made during a transaction if an error occurs before COMMIT.

---

## Practical Example

```sql
BEGIN TRANSACTION;

UPDATE accounts
SET balance = balance - 1000
WHERE account_id = 101;

ROLLBACK;
```

---

## Common Mistakes

- Attempting ROLLBACK after COMMIT
- Forgetting to handle failures

---

## Expected Interview Questions

- What is ROLLBACK?
- When should ROLLBACK be used?
- Can ROLLBACK undo committed changes?

--------------------------------------------------

# 🧠 3. Why COMMIT and ROLLBACK are Important ⭐

## What is it

COMMIT and ROLLBACK ensure reliable transaction processing and maintain database consistency.

---

## Key Components

- Data integrity
- Error recovery
- Safe transactions
- Prevent partial updates

---

## How to Answer (Interview Style)

COMMIT and ROLLBACK ensure that transactions either complete successfully or leave the database unchanged if an error occurs.

---

## Practical Example

```text
Successful bank transfer → COMMIT

Failed bank transfer → ROLLBACK
```

---

## Common Mistakes

- Ignoring transaction handling
- Saving incomplete transactions

---

## Expected Interview Questions

- Why are COMMIT and ROLLBACK important?
- Give a real-world example.

--------------------------------------------------

# 🧠 4. COMMIT Syntax ⭐

## What is it

Standard syntax for saving a successful transaction.

---

## Key Components

- BEGIN TRANSACTION
- SQL statements
- COMMIT

---

## How to Answer (Interview Style)

COMMIT permanently saves all successful changes made within a transaction.

---

## Practical Example

```sql
BEGIN TRANSACTION;

INSERT INTO users(name, email)
VALUES('John', 'john@email.com');

COMMIT;
```

---

## Another Example

```sql
BEGIN TRANSACTION;

UPDATE products
SET stock = stock - 1
WHERE product_id = 10;

COMMIT;
```

---

## Common Mistakes

- Executing COMMIT before all operations finish
- Forgetting COMMIT after successful execution

---

## Expected Interview Questions

- COMMIT syntax?
- What happens after COMMIT?

--------------------------------------------------

# 🧠 5. ROLLBACK Syntax ⭐

## What is it

Standard syntax for cancelling a transaction.

---

## Key Components

- BEGIN TRANSACTION
- SQL statements
- ROLLBACK

---

## How to Answer (Interview Style)

ROLLBACK cancels all uncommitted changes and restores the database to its previous consistent state.

---

## Practical Example

```sql
BEGIN TRANSACTION;

DELETE FROM employees
WHERE employee_id = 5;

ROLLBACK;
```

---

## Another Example

```sql
BEGIN TRANSACTION;

UPDATE orders
SET status = 'Delivered'
WHERE order_id = 1001;

ROLLBACK;
```

---

## Common Mistakes

- Forgetting BEGIN TRANSACTION
- Expecting ROLLBACK to undo committed changes

---

## Expected Interview Questions

- ROLLBACK syntax?
- What happens after ROLLBACK?

--------------------------------------------------

# 🧠 6. COMMIT vs ROLLBACK ⭐

## Difference

| COMMIT | ROLLBACK |
|---------|----------|
| Saves changes permanently | Cancels changes |
| Ends transaction | Ends transaction |
| Cannot be undone | Restores previous state |
| Used after success | Used after failure |

---

## How to Answer (Interview Style)

COMMIT permanently saves transaction changes, whereas ROLLBACK discards all uncommitted changes and restores the previous database state.

---

## Practical Example

```text
Successful Payment → COMMIT

Failed Payment → ROLLBACK
```

---

## Common Mistakes

- Confusing COMMIT with SAVEPOINT
- Using ROLLBACK after COMMIT

---

## Expected Interview Questions

- COMMIT vs ROLLBACK?
- Which command permanently saves data?

--------------------------------------------------

# 🧠 7. SAVEPOINT ⭐

## What is it

SAVEPOINT creates a checkpoint inside a transaction, allowing partial rollback instead of cancelling the entire transaction.

---

## Key Components

- Checkpoint
- Partial rollback
- Long transactions
- Error recovery

---

## How to Answer (Interview Style)

SAVEPOINT creates an intermediate checkpoint inside a transaction so that SQL can roll back only part of the transaction instead of the entire transaction.

---

## Practical Example

```sql
BEGIN TRANSACTION;

UPDATE accounts
SET balance = balance - 1000
WHERE account_id = 101;

SAVEPOINT transfer_step;

UPDATE accounts
SET balance = balance + 1000
WHERE account_id = 102;

ROLLBACK TO transfer_step;

COMMIT;
```

---

## Common Mistakes

- Assuming SAVEPOINT permanently saves data
- Forgetting SAVEPOINT names

---

## Expected Interview Questions

- What is SAVEPOINT?
- SAVEPOINT vs ROLLBACK?
- Why is SAVEPOINT useful?

--------------------------------------------------

# 🧠 8. Real-Time Testing Scenarios ⭐

## Banking Applications

```text
Commit successful fund transfers and rollback failed transfers.
```

---

## E-Commerce Applications

```text
Commit successful orders and rollback failed payment transactions.
```

---

## User Management Systems

```text
Rollback user registration if role assignment fails.
```

---

## Automation Testing

```text
Validate database rollback when an API transaction fails.
```

--------------------------------------------------

# 🧠 9. Performance Considerations ⭐

## What is it

Improper transaction handling can reduce performance and increase database locking.

---

## Key Components

- Transaction duration
- Locking
- Deadlocks
- Resource usage
- Concurrency

---

## Best Practices

- Commit transactions immediately after success.
- Rollback immediately after failures.
- Keep transactions short.
- Avoid unnecessary locks.
- Use SAVEPOINT for long transactions.

---

## How to Answer (Interview Style)

Efficient use of COMMIT and ROLLBACK minimizes locking, improves concurrency, and prevents unnecessary resource consumption.

---

## Practical Example

```text
Commit immediately after updating inventory to release database locks quickly.
```

---

## Common Mistakes

- Long-running transactions
- Forgetting COMMIT
- Ignoring deadlocks
- Leaving transactions open

---

## Expected Interview Questions

- How do COMMIT and ROLLBACK affect performance?
- Why should transactions be short?

--------------------------------------------------

# 🧠 10. Common Mistakes ⭐

- Forgetting COMMIT
- Using ROLLBACK after COMMIT
- Ignoring SAVEPOINT
- Long-running transactions
- Leaving transactions open
- Poor transaction handling

--------------------------------------------------

# 🧠 11. Common Interview Questions ⭐

- What is COMMIT?
- What is ROLLBACK?
- COMMIT vs ROLLBACK?
- What is SAVEPOINT?
- Can ROLLBACK undo COMMIT?
- Why are COMMIT and ROLLBACK important?
- Real-world use cases?
- Best practices for transaction management?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. COMMIT Syntax ⭐
2. ROLLBACK Syntax ⭐
3. COMMIT vs ROLLBACK ⭐
4. SAVEPOINT ⭐
5. Banking Transaction Example ⭐
6. Error Recovery ⭐
7. Transaction Best Practices ⭐

--------------------------------------------------
