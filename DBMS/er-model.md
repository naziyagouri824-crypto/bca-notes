# 🗄️ DBMS — ER Model

The **Entity-Relationship (ER) Model** is a high-level conceptual model used to design the structure of a database.

It represents:

* Entities
* Attributes
* Relationships
* Constraints

ER diagrams are commonly used during the database design process.

## 📌 Entity

An **entity** is a real-world object or concept that can be uniquely identified.

Examples:

* Student
* Teacher
* Course
* Employee
* Department

### Entity Set

A collection of similar entities is called an **entity set**.

Example:

```text
Student
 ├── Student 101
 ├── Student 102
 └── Student 103
```

Here, all students together form a Student entity set.

## 🏷️ Attributes

An attribute describes a property or characteristic of an entity.

For example, a Student entity may have:

```text
Student
 ├── Student_ID
 ├── Name
 ├── Age
 ├── Course
 └── Email
```

### Types of Attributes

#### 1. Simple Attribute

Cannot be divided into smaller parts.

Example:

```text
Age
```

#### 2. Composite Attribute

Can be divided into smaller components.

Example:

```text
Name
 ├── First Name
 ├── Middle Name
 └── Last Name
```

#### 3. Single-Valued Attribute

Has only one value for an entity.

Example:

```text
Student_ID
```

#### 4. Multi-Valued Attribute

Can have multiple values.

Example:

```text
Phone_Number
```

A person may have more than one phone number.

#### 5. Derived Attribute

Its value can be calculated from another attribute.

Example:

```text
Date_of_Birth → Age
```

## 🔑 Keys

A key is an attribute or set of attributes used to identify records uniquely.

### Primary Key

A primary key uniquely identifies each record in a table.

Example:

```text
Student_ID
```

Two students cannot have the same Student_ID.

### Candidate Key

A candidate key is an attribute or combination of attributes that can uniquely identify a record and can potentially become the primary key.

### Composite Key

A composite key consists of two or more attributes used together to uniquely identify a record.

Example:

```text
Student_ID + Course_ID
```

## 🔗 Relationship

A relationship represents an association between two or more entities.

Example:

```text
Student ─── Enrolls ─── Course
```

Here:

* Student = Entity
* Course = Entity
* Enrolls = Relationship

## 📊 Types of Relationships

### 1. One-to-One (1:1)

One entity is related to only one entity.

Example:

```text
Person ─── Passport
```

One person has one passport.

### 2. One-to-Many (1:N)

One entity can be related to many entities.

Example:

```text
Department ─── Employees
```

One department can have many employees.

### 3. Many-to-Many (M:N)

Many entities can be related to many entities.

Example:

```text
Student ─── Courses
```

A student can enroll in many courses, and a course can have many students.

## 📐 Mapping Constraints

Mapping constraints specify how many entities can participate in a relationship.

The two important types are:

### Cardinality

Cardinality specifies the number of entities that can participate in a relationship.

Common cardinalities:

* 1:1
* 1:N
* N:1
* M:N

### Participation Constraint

Participation specifies whether every entity must participate in a relationship.

#### Total Participation

Every entity must participate in the relationship.

#### Partial Participation

Only some entities participate in the relationship.

## 🖼️ ER Diagram Symbols

Common ER diagram symbols include:

```text
Rectangle  → Entity

Oval       → Attribute

Diamond    → Relationship

Double Oval → Multi-valued Attribute

Underlined Attribute → Key Attribute
```

Example:

```text
        (Name)
          |
          |
(Student_ID) —— [ STUDENT ]
          |
       (Course)
```

## 🌳 Generalization

Generalization is a **bottom-up approach** in which common characteristics of multiple entities are combined into a higher-level entity.

Example:

```text
       Employee
          ▲
     ┌────┴────┐
   Teacher   Clerk
```

Teacher and Clerk are specialized types of Employee.

## 🔍 Specialization

Specialization is a **top-down approach** in which a higher-level entity is divided into more specific entities.

Example:

```text
       Employee
          |
     ┌────┴────┐
     ↓         ↓
  Teacher     Clerk
```

## 🔗 Aggregation

Aggregation is used when a relationship itself needs to participate in another relationship.

It allows a relationship set to be treated as a higher-level entity.

Example:

```text
Employee ─── Works_On ─── Project
                 |
                 |
              Monitored
                 |
              Manager
```

Here, the `Works_On` relationship can participate in another relationship.

## 🗂️ ER Model Example — College Database

A simple college database may contain:

```text
Student
   |
 Enrolls
   |
 Course
```

Student attributes:

* Student_ID
* Name
* Email
* Course

Course attributes:

* Course_ID
* Course_Name
* Credits

The `Enrolls` relationship connects students with courses.

## 🎯 Learning Goals

* Understand the ER model
* Identify entities and attributes
* Understand different types of attributes
* Learn keys
* Understand relationships
* Learn cardinality and participation constraints
* Understand ER diagram symbols
* Understand specialization and generalization
* Understand aggregation
* Design basic ER models for databases

---

**Author:** Naziya Gouri
**Course:** BCA – 3rd Semester
