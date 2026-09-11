# ☕ Object-Oriented Programming in Java

Object-Oriented Programming (OOP) is a programming approach based on **objects and classes**.

Java is an object-oriented programming language and supports important OOP concepts such as encapsulation, inheritance, polymorphism, and abstraction.

## 📌 Class

A class is a blueprint or template used to create objects.

Example:

```java
class Student {
    String name;
    int age;
}
```

Here, `Student` is a class.

## 📌 Object

An object is an instance of a class.

Example:

```java
Student student1 = new Student();
```

Here, `student1` is an object of the `Student` class.

## 🔐 Encapsulation

Encapsulation means wrapping data and methods together inside a class.

It also helps control access to data.

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

The `private` variable cannot be accessed directly from outside the class.

## 🛡️ Data Hiding

Data hiding means restricting direct access to the internal data of a class.

It is commonly achieved using the `private` access modifier.

```java
class Account {
    private double balance;
}
```

## 🌳 Inheritance

Inheritance allows one class to acquire properties and methods of another class.

The existing class is called the **parent/superclass**, while the new class is called the **child/subclass**.

Example:

```java
class Animal {
    void eat() {
        System.out.println("Eating...");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Barking...");
    }
}
```

Here, `Dog` inherits the `eat()` method from `Animal`.

## 🔄 Polymorphism

Polymorphism means **one name, many forms**.

In Java, polymorphism is mainly achieved through:

* Method overloading
* Method overriding

## ➕ Method Overloading

Method overloading occurs when multiple methods have the same name but different parameters.

Example:

```java
class Calculator {

    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }
}
```

Both methods are named `add()`, but their parameter lists are different.

This is an example of **compile-time polymorphism**.

## 🔁 Method Overriding

Method overriding occurs when a child class provides its own implementation of a method already defined in the parent class.

Example:

```java
class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Dog barks");
    }
}
```

Here, `Dog` provides its own version of `sound()`.

This is an example of **runtime polymorphism**.

## 🎭 Abstraction

Abstraction means hiding implementation details and showing only the essential features.

Java supports abstraction using:

* Abstract classes
* Interfaces

Example:

```java
abstract class Animal {

    abstract void sound();

    void sleep() {
        System.out.println("Sleeping...");
    }
}
```

## 🧱 Constructor

A constructor is a special method used to initialize an object.

It has the same name as the class and does not have a return type.

Example:

```java
class Student {

    String name;

    Student(String name) {
        this.name = name;
    }
}
```

Creating an object:

```java
Student s1 = new Student("Naziya");
```

## 🧩 Four Main Pillars of OOP

| Concept       | Meaning                                 |
| ------------- | --------------------------------------- |
| Encapsulation | Wrapping data and methods together      |
| Inheritance   | Acquiring properties from another class |
| Polymorphism  | One name, many forms                    |
| Abstraction   | Hiding implementation details           |

## 🎯 Advantages of OOP

* Code reusability
* Better organization
* Easier maintenance
* Data security
* Flexibility
* Reduced code duplication

## 🎯 Learning Goals

* Understand classes and objects
* Understand encapsulation and data hiding
* Learn inheritance
* Understand polymorphism
* Practice method overloading and overriding
* Understand abstraction
* Build programs using OOP concepts

---

**Author:** Naziya Gouri
**Course:** BCA – 3rd Semester
