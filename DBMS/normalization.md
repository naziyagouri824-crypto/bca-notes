# 🗄️ DBMS — Normalization

**Normalization** is a database design technique used to organize data into tables in order to reduce data redundancy and avoid data anomalies.

The main goals of normalization are:

* Reduce duplicate data
* Improve data consistency
* Avoid insertion anomalies
* Avoid update anomalies
* Avoid deletion anomalies
* Improve database structure

## 📌 Data Redundancy

Data redundancy means storing the same data unnecessarily in multiple places.

Example:

| Student_ID | Student_Name | Course |
| ---------- | ------------ | ------ |
| 101        | Ali          | BCA    |
| 102        | Sara         | BCA    |
| 103        | John         | BCA    |

If the same course information is repeatedly stored with every student, unnecessary duplication may occur.

Normalization helps reduce such redundancy.

---

# 1️⃣ First Normal Form (1NF)

A table is in **1NF** when:

* Each column contains atomic values.
* There are no repeating groups.
* Each cell contains a single value.

### ❌ Not in 1NF

| Student_ID | Name | Phone      |
| ---------- | ---- | ---------- |
| 101        | Ali  | 9876, 8765 |

The Phone column contains multiple values.

### ✅ In 1NF

| Student_ID | Name | Phone |
| ---------- | ---- | ----- |
| 101        | Ali  | 9876  |
| 101        | Ali  | 8765  |

Each cell now contains a single value.

---

# 2️⃣ Second Normal Form (2NF)

A table is in **2NF** when:

1. It is already in 1NF.
2. It has no **partial dependency**.

### Partial Dependency

Partial dependency occurs when a non-key attribute depends only on part of a composite primary key.

Example:

```text
(Student_ID, Course_ID) → Grade
Student_ID → Student_Name
```

Here, `Student_Name` depends only on `Student_ID`, not on the complete composite key.

This is a partial dependency.

To achieve 2NF, separate the dependent data into different tables.

### Student Table

| Student_ID | Student_Name |
| ---------- | ------------ |
| 101        | Ali          |
| 102        | Sara         |

### Enrollment Table

| Student_ID | Course_ID | Grade |
| ---------- | --------- | ----- |
| 101        | C01       | A     |
| 102        | C02       | B     |

---

# 3️⃣ Third Normal Form (3NF)

A table is in **3NF** when:

1. It is already in 2NF.
2. It has no **transitive dependency**.

### Transitive Dependency

A transitive dependency occurs when a non-key attribute depends on another non-key attribute.

Example:

```text
Student_ID → Department_ID
Department_ID → Department_Name
```

Therefore:

```text
Student_ID → Department_Name
```

The Department_Name depends indirectly on Student_ID through Department_ID.

To remove this dependency, separate the department information.

### Student Table

| Student_ID | Student_Name | Department_ID |
| ---------- | ------------ | ------------- |
| 101        | Ali          | D01           |
| 102        | Sara         | D02           |

### Department Table

| Department_ID | Department_Name  |
| ------------- | ---------------- |
| D01           | Computer Science |
| D02           | Commerce         |

---

# 4️⃣ Boyce-Codd Normal Form (BCNF)

**BCNF** is a stronger version of 3NF.

A relation is in BCNF if, for every non-trivial functional dependency:

```text
X → Y
```

`X` must be a **super key**.

In simple words:

> Every determinant must be a candidate key or a super key.

BCNF helps remove certain types of redundancy that may still exist in a table satisfying 3NF.

---

# 5️⃣ Fourth Normal Form (4NF)

A relation is in **4NF** when:

1. It is already in BCNF.
2. It has no non-trivial **multivalued dependency**.

### Multivalued Dependency

A multivalued dependency occurs when one attribute determines multiple independent values of another attribute.

Example:

A student may have multiple hobbies and multiple languages.

If these are independent, storing them together can create unnecessary combinations.

Separating them into different relations can help achieve 4NF.

### Student-Hobby

| Student_ID | Hobby   |
| ---------- | ------- |
| 101        | Cricket |
| 101        | Music   |

### Student-Language

| Student_ID | Language |
| ---------- | -------- |
| 101        | English  |
| 101        | Hindi    |

---

# 6️⃣ Fifth Normal Form (5NF)

**5NF** is also called **Project-Join Normal Form (PJ/NF)**.

A relation is in 5NF when:

* It is already in 4NF.
* It cannot be further decomposed without losing information.
* All join dependencies are implied by candidate keys.

5NF mainly deals with complex join dependencies.

---

# 📊 Normalization Summary

| Normal Form | Main Concept                     |
| ----------- | -------------------------------- |
| 1NF         | Atomic values                    |
| 2NF         | Remove partial dependency        |
| 3NF         | Remove transitive dependency     |
| BCNF        | Every determinant is a super key |
| 4NF         | Remove multivalued dependency    |
| 5NF         | Remove join dependency           |

## 🔄 Normalization Flow

```text
Unnormalized Data
       ↓
      1NF
       ↓
      2NF
       ↓
      3NF
       ↓
     BCNF
       ↓
      4NF
       ↓
      5NF
```

## 🎯 Advantages of Normalization

* Reduces data redundancy
* Improves data consistency
* Makes database structure organized
* Reduces update problems
* Reduces insertion problems
* Reduces deletion problems
* Makes database maintenance easier

## ⚠️ Disadvantages

Excessive normalization can result in:

* More tables
* More joins
* More complex queries
* Potentially slower retrieval for some workloads

Therefore, database design should balance normalization with practical performance requirements.

## 🎯 Learning Goals

* Understand the purpose of normalization
* Understand data redundancy
* Learn 1NF and atomic values
* Understand partial dependency and 2NF
* Understand transitive dependency and 3NF
* Learn BCNF
* Understand multivalued dependency and 4NF
* Understand join dependency and 5NF

---

**Author:** Naziya Gouri
**Course:** BCA – 3rd Semester
