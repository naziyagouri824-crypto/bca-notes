# C Programming Notes

C is a general-purpose programming language developed by **Dennis Ritchie** at Bell Labs.

It is widely used for system programming, embedded systems, operating systems, and learning programming fundamentals.

## 📌 Features of C

* Fast and efficient
* Portable
* Structured programming language
* Supports pointers
* Provides low-level memory access
* Suitable for system programming

## 🧩 Basic Structure of a C Program

```c
#include <stdio.h>

int main() {
    printf("Hello, World!");
    return 0;
}
```

### Explanation

* `#include <stdio.h>` → Includes the standard input/output library.
* `main()` → Starting point of the program.
* `printf()` → Displays output on the screen.
* `return 0` → Indicates successful program execution.

## 📦 Variables

A variable is a named memory location used to store data.

Example:

```c
int age = 19;
float marks = 85.5;
char grade = 'A';
```

## 🔢 Data Types

Common data types in C:

| Data Type | Purpose               | Example   |
| --------- | --------------------- | --------- |
| `int`     | Integer values        | `10`      |
| `float`   | Decimal values        | `10.5`    |
| `double`  | Larger decimal values | `25.6789` |
| `char`    | Single character      | `'A'`     |

## ➕ Operators

### Arithmetic Operators

```text
+   Addition
-   Subtraction
*   Multiplication
/   Division
%   Modulus
```

Example:

```c
int a = 10;
int b = 3;

printf("%d", a + b);
```

## 🔄 Conditional Statements

Conditional statements are used to make decisions.

### `if` Statement

```c
int age = 18;

if (age >= 18) {
    printf("Eligible");
}
```

### `if-else`

```c
int number = 10;

if (number % 2 == 0) {
    printf("Even");
} else {
    printf("Odd");
}
```

## 🔁 Loops

Loops are used to repeat a block of code.

### `for` Loop

```c
for (int i = 1; i <= 5; i++) {
    printf("%d\n", i);
}
```

### `while` Loop

```c
int i = 1;

while (i <= 5) {
    printf("%d\n", i);
    i++;
}
```

## 🔧 Functions

A function is a block of code designed to perform a particular task.

Example:

```c
int add(int a, int b) {
    return a + b;
}
```

Calling the function:

```c
int result = add(5, 3);
printf("%d", result);
```

## 📍 Arrays

An array stores multiple values of the same data type.

Example:

```c
int marks[5] = {80, 75, 90, 85, 88};
```

Array elements are accessed using an index starting from `0`.

```c
printf("%d", marks[0]);
```

## 🎯 Learning Goals

* Understand C programming fundamentals
* Practice variables and data types
* Learn operators and expressions
* Understand conditional statements
* Practice loops
* Learn functions and arrays
* Build a strong programming foundation

---

**Author:** Naziya Gouri
**Course:** BCA
