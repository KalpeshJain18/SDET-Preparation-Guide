# 🚀 SQL FOR SDET → SQL Constraints ⭐

SQL Constraints are one of the MOST IMPORTANT SQL concepts for:
- Data integrity
- Backend validation
- Database consistency
- Real-time production systems

Interviewers ask this in:
- SQL interview rounds
- Backend testing discussions
- Database design interviews
- SDET technical rounds

--------------------------------------------------

# 🎯 Topics Covered

1. What are SQL Constraints
2. Why Constraints are Important
3. NOT NULL Constraint
4. UNIQUE Constraint
5. PRIMARY KEY Constraint
6. FOREIGN KEY Constraint
7. CHECK Constraint
8. DEFAULT Constraint
9. Real-Time Testing Scenarios
10. Common Mistakes
11. Common Interview Questions

--------------------------------------------------

# 🧠 1. What are SQL Constraints

## What is it

Constraints are rules applied on database columns.

---

## Key Components

- Data validation
- Integrity enforcement
- Business rules

---

## How to Answer (Interview Style)

SQL constraints are rules used to maintain data accuracy and integrity in database tables.

---

## Practical Example

```sql
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100) NOT NULL
);
```

---

## Common Mistakes

- Ignoring constraint rules
- Weak schema design

---

## Expected Interview Questions

- What are SQL constraints?
- Why constraints important?
- Real-time examples?

--------------------------------------------------

# 🧠 2. Why Constraints are Important ⭐

## What is it

Used for maintaining valid business data.

---

## Key Components

- Data consistency
- Validation enforcement
- Database reliability

---

## How to Answer (Interview Style)

Constraints help prevent invalid or inconsistent data from entering the database.

---

## Practical Example

```text
Prevent duplicate email registrations
```

---

## Common Mistakes

- No validation rules

---

## Expected Interview Questions

- Why constraints used?
- Real-time usage?

--------------------------------------------------

# 🧠 3. NOT NULL Constraint ⭐

## What is it

Prevents NULL values in columns.

---

## Key Components

- Mandatory fields
- Data completeness

---

## How to Answer (Interview Style)

NOT NULL ensures mandatory fields always contain values.

---

## Practical Example

```sql
CREATE TABLE users (
    username VARCHAR(50) NOT NULL
);
```

---

## Common Mistakes

- Allowing important fields to remain NULL

---

## Expected Interview Questions

- NOT NULL usage?
- Real-time examples?

--------------------------------------------------

# 🧠 4. UNIQUE Constraint ⭐

## What is it

Prevents duplicate values.

---

## Key Components

- Uniqueness validation
- Duplicate prevention

---

## How to Answer (Interview Style)

UNIQUE constraint ensures column values remain distinct.

---

## Practical Example

```sql
CREATE TABLE users (
    email VARCHAR(100) UNIQUE
);
```

---

## Common Mistakes

- Confusing UNIQUE with PRIMARY KEY

---

## Expected Interview Questions

- UNIQUE vs PRIMARY KEY?
- Duplicate handling?

--------------------------------------------------

# 🧠 5. PRIMARY KEY Constraint ⭐

## What is it

Uniquely identifies each record.

---

## Key Components

- Unique identification
- No NULL values

---

## How to Answer (Interview Style)

PRIMARY KEY uniquely identifies every row in a table.

---

## Practical Example

```sql
CREATE TABLE employees (
    id INT PRIMARY KEY
);
```

---

## Common Mistakes

- Multiple primary keys misunderstanding

---

## Expected Interview Questions

- What is PRIMARY KEY?
- Why PRIMARY KEY important?

--------------------------------------------------

# 🧠 6. FOREIGN KEY Constraint ⭐

## What is it

Maintains relationships between tables.

---

## Key Components

- Referential integrity
- Table relationships

---

## How to Answer (Interview Style)

FOREIGN KEY links records between related tables.

---

## Practical Example

```sql
CREATE TABLE orders (
    user_id INT,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

---

## Common Mistakes

- Invalid reference mapping

---

## Expected Interview Questions

- What is FOREIGN KEY?
- Referential integrity?

--------------------------------------------------

# 🧠 7. CHECK Constraint ⭐

## What is it

Validates values using conditions.

---

## Key Components

- Business rule validation
- Conditional restrictions

---

## How to Answer (Interview Style)

CHECK constraint ensures values satisfy specified conditions.

---

## Practical Example

```sql
CREATE TABLE employees (
    age INT CHECK (age >= 18)
);
```

---

## Common Mistakes

- Weak validation conditions

---

## Expected Interview Questions

- CHECK constraint usage?
- Real-time examples?

--------------------------------------------------

# 🧠 8. DEFAULT Constraint ⭐

## What is it

Provides default values automatically.

---

## Key Components

- Default assignment
- Automatic values

---

## How to Answer (Interview Style)

DEFAULT constraint assigns predefined values when no value is provided.

---

## Practical Example

```sql
CREATE TABLE employees (
    status VARCHAR(20) DEFAULT 'Active'
);
```

---

## Common Mistakes

- Wrong default value assumptions

---

## Expected Interview Questions

- DEFAULT constraint usage?
- Real-time examples?

--------------------------------------------------

# 🧠 9. Real-Time Testing Scenarios ⭐

## Banking Applications

```text
Prevent duplicate account numbers
```

---

## E-Commerce Applications

```text
Validate mandatory order details
```

---

## User Management Systems

```text
Ensure unique email registration
```

---

## Automation Testing

```text
Validate DB constraints during API testing
```

--------------------------------------------------

# 🧠 10. Common Mistakes ⭐

- Ignoring integrity rules
- Weak validation design
- Confusing UNIQUE and PRIMARY KEY
- Invalid foreign key mapping
- Missing mandatory fields

--------------------------------------------------

# 🧠 11. Common Interview Questions ⭐

- What are SQL constraints?
- UNIQUE vs PRIMARY KEY?
- PRIMARY KEY vs FOREIGN KEY?
- CHECK constraint usage?
- DEFAULT constraint examples?
- Real-time usage examples?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. NOT NULL ⭐
2. UNIQUE Constraint ⭐
3. PRIMARY KEY ⭐
4. FOREIGN KEY ⭐
5. CHECK Constraint ⭐

--------------------------------------------------
