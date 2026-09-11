# ☕ Java Basics

Java is a high-level, object-oriented, class-based programming language designed to be portable, secure, and widely used for application development.

## 📌 Features of Java

Some important features of Java are:

* Simple
* Object-Oriented
* Platform Independent
* Secure
* Robust
* Portable
* Multithreaded
* High Performance

## ⚙️ How Java Works

Java follows the concept of **Write Once, Run Anywhere**.

The basic process is:

```text
Java Source Code
       ↓
    Compiler
       ↓
   Bytecode
       ↓
      JVM
       ↓
   Machine Code
```

A Java program is written in a `.java` file.

The Java compiler converts the source code into **bytecode**, which is stored in a `.class` file.

The **JVM (Java Virtual Machine)** executes the bytecode.

## 🧠 JVM

JVM stands for **Java Virtual Machine**.

It is responsible for executing Java bytecode and making Java platform independent.

## ☕ Simple Java Program

```java
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

### Explanation

* `class` defines a class.
* `HelloWorld` is the class name.
* `main()` is the starting point of program execution.
* `System.out.println()` prints output on the screen.

## 📦 Variables

A variable is a named memory location used to store data.

Example:

```java
int age = 19;
double marks = 85.5;
char grade = 'A';
```

## 🔢 Data Types

Java data types are divided into two major categories:

### Primitive Data Types

* `byte`
* `short`
* `int`
* `long`
* `float`
* `double`
* `char`
* `boolean`

Example:

```java
int age = 19;
double percentage = 85.5;
char grade = 'A';
boolean passed = true;
```

## 🔄 Type Casting

Type casting means converting a value from one data type to another.

### Widening Casting

Smaller data type → larger data type.

```java
int number = 10;
double value = number;
```

### Narrowing Casting

Larger data type → smaller data type.

```java
double value = 10.5;
int number = (int) value;
```

## 🔐 Data Hiding

Data hiding means restricting direct access to the internal data of an object.

It is commonly achieved using access modifiers such as `private`.

Example:

```java
class Student {
    private int marks;
}
```

## 📦 Encapsulation

Encapsulation means wrapping data and methods together inside a class.

Example:

```java
class Student {
    private String name;

    public void setName(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }
}
```

## 🔢 Operators

Java provides different types of operators.

### Arithmetic Operators

```text
+   Addition
-   Subtraction
*   Multiplication
/   Division
%   Modulus
```

### Relational Operators

```text
==   Equal to
!=   Not equal to
>    Greater than
<    Less than
>=   Greater than or equal to
<=   Less than or equal to
```

### Logical Operators

```text
&&   Logical AND
||   Logical OR
!    Logical NOT
```

### Assignment Operators

```text
=    Assignment
+=   Add and assign
-=   Subtract and assign
*=   Multiply and assign
/=   Divide and assign
```

### Increment and Decrement

```text
++   Increment
--   Decrement
```

## 🎯 Learning Goals

* Understand Java fundamentals
* Learn Java program structure
* Understand JVM and bytecode
* Practice variables and data types
* Learn operators
* Understand type casting
* Understand data hiding and encapsulation
* Build Java programs using OOP concepts

---

**Author:** Naziya Gouri
**Course:** BCA – 3rd Semester
