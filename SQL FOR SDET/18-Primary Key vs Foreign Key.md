# 🚀 SQL FOR SDET → Primary Key vs Foreign Key ⭐

Primary Key and Foreign Key are one of the MOST IMPORTANT SQL concepts for:
- Table relationships
- Database design
- Backend validation
- Real-time production systems

Interviewers ask this in:
- SQL interview rounds
- Database design discussions
- Backend testing interviews
- SDET technical rounds

--------------------------------------------------

# 🎯 Topics Covered

1. What is Primary Key
2. What is Foreign Key
3. Why Keys are Important
4. Primary Key Features
5. Foreign Key Features
6. Primary Key vs Foreign Key
7. Relationships between Tables
8. Real-Time Testing Scenarios
9. Common Mistakes
10. Common Interview Questions

--------------------------------------------------

# 🧠 1. What is Primary Key

## What is it

Primary Key uniquely identifies each row in a table.

---

## Key Components

- Unique values
- No NULL values
- One primary key per table

---

## How to Answer (Interview Style)

Primary Key uniquely identifies every record in a database table.

---

## Practical Example

```sql
CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(100)
);
```

---

## Common Mistakes

- Duplicate primary key values
- NULL primary key values

---

## Expected Interview Questions

- What is Primary Key?
- Why Primary Key important?
- Real-time examples?

--------------------------------------------------

# 🧠 2. What is Foreign Key

## What is it

Foreign Key creates relationships between tables.

---

## Key Components

- Referential integrity
- Parent-child relationship
- Table linkage

---

## How to Answer (Interview Style)

Foreign Key connects related tables and maintains referential integrity.

---

## Practical Example

```sql
CREATE TABLE orders (
    order_id INT PRIMARY KEY,
    user_id INT,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

---

## Common Mistakes

- Invalid foreign key references
- Orphan records creation

---

## Expected Interview Questions

- What is Foreign Key?
- Referential integrity?
- Real-time examples?

--------------------------------------------------

# 🧠 3. Why Keys are Important ⭐

## What is it

Keys maintain database integrity and relationships.

---

## Key Components

- Data consistency
- Relationship management
- Validation enforcement

---

## How to Answer (Interview Style)

Keys are important for maintaining unique records and valid table relationships.

---

## Practical Example

```text
User and order relationship management
```

---

## Common Mistakes

- Missing relationship design

---

## Expected Interview Questions

- Why keys important?
- Database integrity examples?

--------------------------------------------------

# 🧠 4. Primary Key Features ⭐

## What is it

Characteristics of primary keys.

---

## Key Components

- Unique
- NOT NULL
- Indexed automatically

---

## How to Answer (Interview Style)

Primary Key must contain unique and non-null values.

---

## Practical Example

```sql
CREATE TABLE employees (
    emp_id INT PRIMARY KEY
);
```

---

## Common Mistakes

- Multiple primary keys confusion

---

## Expected Interview Questions

- Primary Key features?
- Can primary key be NULL?

--------------------------------------------------

# 🧠 5. Foreign Key Features ⭐

## What is it

Characteristics of foreign keys.

---

## Key Components

- References parent table
- Allows duplicate values
- Maintains integrity

---

## How to Answer (Interview Style)

Foreign Key references a primary key in another table.

---

## Practical Example

```sql
FOREIGN KEY (department_id)
REFERENCES departments(id)
```

---

## Common Mistakes

- Reference mismatch

---

## Expected Interview Questions

- Foreign Key features?
- Can Foreign Key contain duplicates?

--------------------------------------------------

# 🧠 6. Primary Key vs Foreign Key ⭐

## Difference

| Primary Key | Foreign Key |
|---|---|
| Unique identifier | Relationship creator |
| No NULL allowed | NULL allowed |
| One per table | Multiple allowed |
| Prevents duplicates | Allows duplicates |

---

## How to Answer (Interview Style)

Primary Key uniquely identifies records, while Foreign Key creates relationships between tables.

---

## Practical Example

```text
users.id → PRIMARY KEY
orders.user_id → FOREIGN KEY
```

---

## Common Mistakes

- Confusing uniqueness behavior

---

## Expected Interview Questions

- Primary Key vs Foreign Key?
- Key relationship examples?

--------------------------------------------------

# 🧠 7. Relationships between Tables ⭐

## What is it

Tables connect through foreign keys.

---

## Key Components

- One-to-One
- One-to-Many
- Many-to-Many

---

## How to Answer (Interview Style)

Foreign Keys help establish relationships between related tables.

---

## Practical Example

```text
One user → Multiple orders
```

---

## Common Mistakes

- Poor relationship design

---

## Expected Interview Questions

- One-to-many relationship?
- Table relationship examples?

--------------------------------------------------

# 🧠 8. Real-Time Testing Scenarios ⭐

## Banking Applications

```text
Customer and transaction relationship
```

---

## E-Commerce Applications

```text
User and order mapping
```

---

## User Management Systems

```text
Role-based relationship validation
```

---

## Automation Testing

```text
Validate referential integrity during API testing
```

--------------------------------------------------

# 🧠 9. Common Mistakes ⭐

- Missing relationship mapping
- Duplicate primary keys
- Invalid foreign key references
- Poor schema design
- Orphan record creation

--------------------------------------------------

# 🧠 10. Common Interview Questions ⭐

- What is Primary Key?
- What is Foreign Key?
- Primary Key vs Foreign Key?
- Can Foreign Key contain NULL?
- One-to-many relationship?
- Real-time usage examples?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. Primary Key ⭐
2. Foreign Key ⭐
3. Referential Integrity ⭐
4. Primary Key vs Foreign Key ⭐
5. Table Relationships ⭐

--------------------------------------------------
