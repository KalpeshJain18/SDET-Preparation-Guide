# 🚀 Java For SDET → Java Basics

This is the foundation of all Java interview preparation.

Interviewers ask this to check:
- Core Java understanding
- Programming fundamentals
- Framework readiness

--------------------------------------------------

Topics Covered:

1. What is Java
2. Features of Java
3. JVM vs JDK vs JRE
4. Java Program Structure
5. Variables & Data Types
6. Operators
7. Conditional Statements
8. Loops
9. Methods in Java
10. Class & Object Basics
11. Static Keyword Basics
12. Common Interview Questions

--------------------------------------------------

# 🧠 1. What is Java

## What is it

Java is an object-oriented, platform-independent programming language used for backend, automation, enterprise, and web applications.

---

## Key Components

- Object-oriented
- Platform independent
- Secure
- Robust
- Portable

---

## How to Answer (Interview Style)

Java is a high-level, object-oriented programming language widely used for enterprise applications, automation frameworks, backend systems, and web development.

---

## Practical Example

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello Kalpesh");
    }
}
```

---

## Common Mistakes

- Saying only “Java is programming language”
- Forgetting platform independence

---

## Expected Interview Questions

- What is Java?
- Why Java is platform independent?
- Why Java is widely used?

--------------------------------------------------

# 🧠 2. Features of Java ⭐

## What is it

Core characteristics that make Java powerful and popular.

---

## Key Components

- Platform Independent
- Object-Oriented
- Secure
- Robust
- Multithreaded
- Portable

---

## How to Answer (Interview Style)

Java is popular because it is object-oriented, platform-independent, secure, robust, and supports multithreading.

---

## Practical Example

```text
Write Once → Run Anywhere
```

---

## Common Mistakes

- Missing important features
- Confusing portability with platform independence

---

## Expected Interview Questions

- What are features of Java?
- Why Java is secure?
- Explain platform independence.

--------------------------------------------------

# 🧠 3. JVM vs JDK vs JRE ⭐

## What is it

Core Java runtime architecture components.

---

## Key Components

### JVM
Runs Java bytecode

### JRE
JVM + libraries required to run Java apps

### JDK
JRE + development tools

---

## How to Answer (Interview Style)

JVM executes Java bytecode, JRE provides runtime environment, and JDK provides development tools required to build Java applications.

---

## Practical Example

```text
.java
 ↓
Compiler
 ↓
.class (Bytecode)
 ↓
JVM Executes
```

---

## Common Mistakes

- Mixing JRE and JDK
- Weak JVM understanding

---

## Expected Interview Questions

- Difference between JVM, JDK, and JRE?
- What is bytecode?
- How Java achieves platform independence?

--------------------------------------------------

# 🧠 4. Java Program Structure

## What is it

Basic structure of a Java program.

---

## Key Components

- Class
- main method
- System.out.println
- Package/import

---

## How to Answer (Interview Style)

Every Java program contains a class and a main method, which acts as the entry point of execution.

---

## Practical Example

```java
public class Demo {

    public static void main(String[] args) {
        System.out.println("Java");
    }
}
```

---

## Common Mistakes

- Wrong main method syntax
- Missing class declaration

---

## Expected Interview Questions

- What is main method?
- Why main method is static?
- Explain Java program flow.

--------------------------------------------------

# 🧠 5. Variables & Data Types

## What is it

Variables store data values in memory.

---

## Key Components

### Primitive Types
- int
- double
- char
- boolean

### Non-Primitive
- String
- Arrays
- Objects

---

## How to Answer (Interview Style)

Variables are memory containers used to store values, and Java supports primitive and non-primitive data types.

---

## Practical Example

```java
int age = 25;
String name = "Kalpesh";
```

---

## Common Mistakes

- Wrong datatype selection
- Uninitialized variables

---

## Expected Interview Questions

- Difference between primitive and non-primitive?
- What are datatypes in Java?
- Why String is non-primitive?

--------------------------------------------------

# 🧠 6. Operators

## What is it

Operators perform operations on variables and values.

---

## Key Components

- Arithmetic
- Relational
- Logical
- Assignment
- Increment/Decrement

---

## How to Answer (Interview Style)

Operators are symbols used to perform arithmetic, logical, relational, and assignment operations in Java.

---

## Practical Example

```java
int a = 10;
int b = 20;

System.out.println(a + b);
```

---

## Common Mistakes

- Confusing == and =
- Incorrect logical conditions

---

## Expected Interview Questions

- Types of operators?
- Difference between == and equals?
- Logical operator examples?

--------------------------------------------------

# 🧠 7. Conditional Statements

## What is it

Used for decision-making in programs.

---

## Key Components

- if
- else
- else-if
- switch

---

## How to Answer (Interview Style)

Conditional statements help execute different code blocks based on conditions.

---

## Practical Example

```java
if(age >= 18) {
   System.out.println("Eligible");
}
```

---

## Common Mistakes

- Incorrect conditions
- Nested if confusion

---

## Expected Interview Questions

- Difference between if and switch?
- When to use switch?
- Nested if example?

--------------------------------------------------

# 🧠 8. Loops

## What is it

Loops execute code repeatedly.

---

## Key Components

- for loop
- while loop
- do-while loop
- enhanced for loop

---

## How to Answer (Interview Style)

Loops are used to repeatedly execute a block of code until a condition becomes false.

---

## Practical Example

```java
for(int i=1; i<=5; i++) {
   System.out.println(i);
}
```

---

## Common Mistakes

- Infinite loops
- Wrong loop conditions

---

## Expected Interview Questions

- Difference between while and do-while?
- What is enhanced for loop?
- Infinite loop example?

--------------------------------------------------

# 🧠 9. Methods in Java ⭐

## What is it

Methods are reusable blocks of code used to perform tasks.

---

## Key Components

- Method declaration
- Parameters
- Return type
- Method calling

---

## How to Answer (Interview Style)

Methods improve code reusability and modularity by grouping related logic into reusable blocks.

---

## Practical Example

```java
public int add(int a, int b) {
   return a + b;
}
```

---

## Common Mistakes

- Wrong return type
- Missing parameters

---

## Expected Interview Questions

- What are methods?
- Difference between parameter and argument?
- Why methods are important?

--------------------------------------------------

# 🧠 10. Class & Object Basics ⭐

## What is it

Class is a blueprint, object is an instance of class.

---

## Key Components

- Class
- Object
- Properties
- Methods

---

## How to Answer (Interview Style)

A class defines properties and behaviors, while objects are runtime instances created from the class.

---

## Practical Example

```java
class Car {
   String color = "Black";
}

Car c = new Car();
```

---

## Common Mistakes

- Confusing class and object
- Incorrect object creation

---

## Expected Interview Questions

- Difference between class and object?
- What is object creation?
- Real-time example of class?

--------------------------------------------------

# 🧠 11. Static Keyword Basics ⭐

## What is it

Static members belong to class instead of object.

---

## Key Components

- Static variable
- Static method
- Shared memory

---

## How to Answer (Interview Style)

Static keyword is used for class-level members shared across all objects.

---

## Practical Example

```java
static int count = 0;
```

---

## Common Mistakes

- Overusing static
- Access confusion

---

## Expected Interview Questions

- What is static keyword?
- Why main method is static?
- Difference between static and non-static?

--------------------------------------------------

# 🧠 12. Common Interview Questions ⭐

- What is Java?
- Features of Java?
- Difference between JVM, JDK, JRE?
- Why Java is platform independent?
- Difference between class and object?
- What is static keyword?
- Why main method is static?
- Difference between primitive and non-primitive?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. JVM vs JDK vs JRE ⭐
2. Methods in Java ⭐
3. Class & Object ⭐
4. Static Keyword ⭐
5. Features of Java ⭐

--------------------------------------------------
