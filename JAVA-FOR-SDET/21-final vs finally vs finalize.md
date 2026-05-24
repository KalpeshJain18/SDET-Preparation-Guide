# 🚀 Java For SDET → final vs finally vs finalize

This is one of the MOST ASKED core Java interview topics.

Interviewers ask this in:
- Java core rounds
- Exception handling discussions
- JVM interviews
- Product companies

Especially important for:
- OOPS concepts
- Exception handling
- Memory management basics

--------------------------------------------------

Topics Covered:

1. What is final Keyword
2. What is finally Block
3. What is finalize() Method
4. final vs finally vs finalize
5. final Variable
6. final Method
7. final Class
8. finally Block Usage
9. finalize() and Garbage Collection
10. Real-Time Framework Usage
11. Common Mistakes
12. Common Interview Questions

--------------------------------------------------

# 🧠 1. What is final Keyword

## What is it

final keyword is used to restrict modifications.

---

## Key Components

- Constant variables
- Method restriction
- Inheritance restriction

---

## How to Answer (Interview Style)

final keyword is used to make variables constant, methods non-overridable, and classes non-inheritable.

---

## Practical Example

```java
final int age = 25;
```

---

## Common Mistakes

- Confusing final with finally
- Expecting final variables to change

---

## Expected Interview Questions

- What is final keyword?
- Why final is used?
- Real-time examples?

--------------------------------------------------

# 🧠 2. What is finally Block ⭐

## What is it

finally block is used in exception handling.

---

## Key Components

- Cleanup code
- Resource closing
- Always executes

---

## How to Answer (Interview Style)

finally block executes regardless of exception occurrence and is mainly used for cleanup operations.

---

## Practical Example

```java
try {

}
finally {

}
```

---

## Common Mistakes

- Confusing finally with finalize()

---

## Expected Interview Questions

- What is finally block?
- Why finally is used?
- Does finally always execute?

--------------------------------------------------

# 🧠 3. What is finalize() Method

## What is it

Method called before garbage collection.

---

## Key Components

- Garbage collection
- Cleanup operation
- JVM-managed execution

---

## How to Answer (Interview Style)

finalize() method is invoked by garbage collector before object destruction.

---

## Practical Example

```java
@Override
protected void finalize() {

}
```

---

## Common Mistakes

- Depending on finalize() for critical logic

---

## Expected Interview Questions

- What is finalize()?
- When finalize executes?
- Why finalize is deprecated?

--------------------------------------------------

# 🧠 4. final vs finally vs finalize ⭐

## What is it

Most important comparison topic.

---

## Key Components

### final
Keyword

### finally
Exception handling block

### finalize()
Garbage collection method

---

## How to Answer (Interview Style)

final is a keyword, finally is an exception handling block, and finalize() is a garbage collection method.

---

## Practical Example

```text
final
→ Restriction

finally
→ Cleanup

finalize()
→ GC cleanup
```

---

## Common Mistakes

- Mixing all three concepts

---

## Expected Interview Questions

- Difference between final finally finalize?
- Real-time examples?
- Which is keyword and method?

--------------------------------------------------

# 🧠 5. final Variable ⭐

## What is it

Variable whose value cannot change.

---

## Key Components

- Constant value
- Immutable behavior
- Single assignment

---

## How to Answer (Interview Style)

final variables can only be assigned once and behave like constants.

---

## Practical Example

```java
final double PI = 3.14;
```

---

## Common Mistakes

- Reassigning final variables

---

## Expected Interview Questions

- What is final variable?
- Can final variables change?
- Real-time usage?

--------------------------------------------------

# 🧠 6. final Method ⭐

## What is it

Method that cannot be overridden.

---

## Key Components

- Inheritance restriction
- Fixed implementation
- Security

---

## How to Answer (Interview Style)

final methods prevent method overriding in child classes.

---

## Practical Example

```java
final void show() {

}
```

---

## Common Mistakes

- Trying to override final methods

---

## Expected Interview Questions

- What is final method?
- Why final methods are used?
- Overriding restrictions?

--------------------------------------------------

# 🧠 7. final Class ⭐

## What is it

Class that cannot be inherited.

---

## Key Components

- Inheritance restriction
- Security
- Immutable design

---

## How to Answer (Interview Style)

final classes prevent inheritance and secure implementation logic.

---

## Practical Example

```java
final class Demo {

}
```

---

## Common Mistakes

- Trying to extend final class

---

## Expected Interview Questions

- What is final class?
- Why String class is final?
- Real-time examples?

--------------------------------------------------

# 🧠 8. finally Block Usage ⭐

## What is it

Used for resource cleanup.

---

## Key Components

- File closing
- DB connection cleanup
- Resource management

---

## How to Answer (Interview Style)

finally blocks are commonly used for closing resources like files and database connections.

---

## Practical Example

```java
finally {

   scanner.close();
}
```

---

## Common Mistakes

- Skipping cleanup logic

---

## Expected Interview Questions

- Real-time finally usage?
- Why cleanup is important?
- Resource management?

--------------------------------------------------

# 🧠 9. finalize() and Garbage Collection ⭐

## What is it

Connection between finalize() and JVM garbage collector.

---

## Key Components

- Object cleanup
- JVM lifecycle
- GC behavior

---

## How to Answer (Interview Style)

finalize() may execute before garbage collection, but execution timing is not guaranteed.

---

## Practical Example

```text
Object unused
→ GC triggered
→ finalize()
```

---

## Common Mistakes

- Assuming finalize always runs

---

## Expected Interview Questions

- finalize and GC relation?
- Why finalize is unreliable?
- Modern alternatives?

--------------------------------------------------

# 🧠 10. Real-Time Framework Usage ⭐

## Selenium Framework

```text
Cleanup browser sessions
```

---

## API Automation

```text
Close API resources
```

---

## Reporting

```text
Protect utility methods
```

---

## Framework Design

```text
Constant configuration values
```

--------------------------------------------------

# 🧠 11. Common Mistakes ⭐

- Confusing final finally finalize
- Reassigning final variables
- Weak exception cleanup understanding
- Depending on finalize()
- Weak garbage collection knowledge

--------------------------------------------------

# 🧠 12. Common Interview Questions ⭐

- Difference between final finally finalize?
- What is final keyword?
- Why finally block is important?
- What is finalize()?
- Why String class is final?
- finalize() and garbage collection relation?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. final vs finally vs finalize ⭐
2. final Variable / Method / Class ⭐
3. finally Block Usage ⭐
4. finalize() and GC ⭐
5. Real-Time Framework Usage ⭐

--------------------------------------------------
