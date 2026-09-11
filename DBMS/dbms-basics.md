# 🗄️ DBMS Basics

DBMS stands for **Database Management System**.

A DBMS is software used to create, store, organize, retrieve, and manage data in a database.

## 📌 What is a Database?

A database is an organized collection of related data that can be easily accessed, managed, and updated.

### Example

A college database may contain:

* Student details
* Teacher details
* Course details
* Marks
* Attendance

## 🎯 Purpose of a Database System

A database system is used to manage large amounts of data efficiently.

Important purposes include:

* Storing data
* Retrieving data
* Updating data
* Reducing data redundancy
* Maintaining data consistency
* Providing data security
* Allowing multiple users to access data

## 📊 Data Abstraction

Data abstraction means **hiding unnecessary implementation details from users** and showing only the required information.

DBMS provides three levels of data abstraction:

### 1. Physical Level

Describes **how data is actually stored** in memory or storage devices.

Example:

How database files and records are physically stored.

### 2. Logical Level

Describes **what data is stored** and the relationships between different data items.

Example:

A Student table may contain:

```text
Student_ID
Name
Course
Marks
```

### 3. View Level

Describes only the part of the database that a particular user needs to see.

Example:

A student may see their marks, while an administrator may see complete student records.

```text
View Level
    ↓
Logical Level
    ↓
Physical Level
```

## 🧩 Data Model

A data model describes how data is structured, stored, and related within a database.

Common types include:

* Hierarchical Model
* Network Model
* Relational Model
* Entity-Relationship Model
* Object-Oriented Model

### Relational Model

The relational model represents data using **tables** consisting of rows and columns.

Example:

| Student_ID | Name | Course |
| ---------- | ---- | ------ |
| 101        | Ali  | BCA    |
| 102        | Sara | BCA    |

## 🔄 Data Independence

Data independence means the ability to change the database structure at one level without requiring changes at the next higher level.

There are two types:

### 1. Physical Data Independence

Changes in the physical storage of data do not affect the logical structure.

Example:

Changing the way database files are stored without changing the tables.

### 2. Logical Data Independence

Changes in the logical structure do not affect the user's views or application programs.

Example:

Adding a new field to a table without changing existing user views.

## 📝 DDL

DDL stands for **Data Definition Language**.

DDL commands are used to define and modify the structure of database objects such as tables.

Common DDL commands:

* `CREATE`
* `ALTER`
* `DROP`
* `TRUNCATE`

Example:

```sql
CREATE TABLE Student (
    id INT,
    name VARCHAR(50)
);
```

## ✏️ DML

DML stands for **Data Manipulation Language**.

DML commands are used to insert, modify, and retrieve data from database tables.

Common DML commands:

* `INSERT`
* `UPDATE`
* `DELETE`
* `SELECT`

Example:

```sql
INSERT INTO Student (id, name)
VALUES (101, 'Naziya');
```

## 👨‍💼 Database Administrator

A **Database Administrator (DBA)** is responsible for managing and maintaining the database system.

### Responsibilities of a DBA

* Database security
* User access management
* Backup and recovery
* Performance monitoring
* Database maintenance
* Managing storage

## 👥 Database Users

Different types of users interact with a database.

### 1. Database Administrator

Manages and controls the database system.

### 2. Application Programmers

Develop applications that interact with the database.

### 3. End Users

Use applications to access database information.

Examples:

* Students
* Teachers
* Bank customers
* Employees

## 🗂️ Database Manager

A database manager is responsible for managing the interaction between applications/users and the database.

It helps with tasks such as:

* Data storage
* Data retrieval
* Data updates
* Transaction management
* Security and access control

## 🎯 Learning Goals

* Understand databases and DBMS
* Understand the purpose of a database system
* Learn the three levels of data abstraction
* Understand different data models
* Understand data independence
* Learn DDL and DML commands
* Understand the role of DBA
* Understand different types of database users

---

**Author:** Naziya Gouri
**Course:** BCA – 3rd Semester
