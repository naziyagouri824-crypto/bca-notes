# JavaScript Notes

JavaScript is a programming language used to make web pages interactive and dynamic.

HTML creates the structure, CSS controls the design, and JavaScript adds functionality and behavior.

## 📌 Why is JavaScript Used?

JavaScript can be used to:

* Handle user interactions
* Change HTML content
* Modify CSS styles
* Validate forms
* Perform calculations
* Create interactive web applications
* Respond to events such as clicks and keyboard input

## 🧩 Variables

Variables are used to store data.

### `let`

Used when the value of a variable may change.

```javascript
let age = 19;
age = 20;
```

### `const`

Used when the variable should not be reassigned.

```javascript
const name = "Naziya";
```

## 📦 Data Types

Common JavaScript data types include:

* String
* Number
* Boolean
* Undefined
* Null
* Object

Example:

```javascript
let name = "Naziya";      // String
let age = 19;             // Number
let isStudent = true;     // Boolean
```

## ➕ Operators

JavaScript supports different types of operators.

### Arithmetic Operators

```text
+   Addition
-   Subtraction
*   Multiplication
/   Division
%   Modulus
```

Example:

```javascript
let result = 10 + 5;
```

## 🔧 Functions

A function is a reusable block of code designed to perform a specific task.

Example:

```javascript
function greet() {
    console.log("Hello!");
}

greet();
```

Functions can also accept parameters.

```javascript
function add(a, b) {
    return a + b;
}

let result = add(5, 3);
```

## 🖱️ Events

JavaScript can respond to events such as:

* Click
* Mouse movement
* Keyboard input
* Form submission
* Page loading

Example:

```javascript
button.addEventListener("click", function() {
    console.log("Button clicked!");
});
```

## 🌐 DOM

DOM stands for **Document Object Model**.

It allows JavaScript to access and modify HTML elements.

Example:

```javascript
const heading = document.getElementById("heading");

heading.textContent = "Hello World";
```

## 🧮 JavaScript in My Calculator Project

In my calculator project, JavaScript is used to handle button clicks and perform calculations.

For example:

```javascript
function appendValue(value) {
    display.value += value;
}
```

This function adds the clicked value to the calculator display.

The calculator also uses functions such as:

```javascript
function clearDisplay() {
    display.value = "";
}
```

and:

```javascript
function deleteLast() {
    display.value = display.value.slice(0, -1);
}
```

These functions demonstrate how JavaScript can make a webpage interactive.

## 🔄 Loops

Loops are used to repeat a block of code.

### `for` Loop

```javascript
for (let i = 1; i <= 5; i++) {
    console.log(i);
}
```

### `while` Loop

```
```
