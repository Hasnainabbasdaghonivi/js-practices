# 📘 JavaScript Notes

Basic to intermediate JavaScript concepts for quick revision.

---

## ✨ Introduction

* **JavaScript (JS)** ek programming language hai jo mainly **web development** mein use hoti hai.
* Ye **browser** aur **server (Node.js)** dono par chal sakti hai.

---

## 🔹 Variables

```js
// var (old way)
var name = "Hasnain";

// let (block scope)
let age = 21;

// const (constant value)
const country = "Pakistan";
```

---

## 🔹 Data Types

1. Primitive: `String`, `Number`, `Boolean`, `Undefined`, `Null`, `Symbol`, `BigInt`
2. Non-Primitive: `Object`, `Array`, `Function`

```js
let str = "Hello";      // String
let num = 42;           // Number
let flag = true;        // Boolean
let arr = [1, 2, 3];    // Array
let obj = {name: "Ali", age: 20}; // Object
```

---

## 🔹 Operators

```js
// Arithmetic
let sum = 5 + 3;
let mul = 5 * 3;

// Comparison
5 > 3   // true
5 == "5" // true (loose compare)
5 === "5" // false (strict compare)

// Logical
true && false // false
true || false // true
!true         // false
```

---

## 🔹 Conditional Statements

```js
let marks = 85;

if (marks >= 90) {
  console.log("Grade A");
} else if (marks >= 50) {
  console.log("Pass");
} else {
  console.log("Fail");
}

// Switch
let day = 2;
switch (day) {
  case 1: console.log("Monday"); break;
  case 2: console.log("Tuesday"); break;
  default: console.log("Other day");
}

// Ternary
let age = 18;
let result = (age >= 18) ? "Adult" : "Minor";
```

---

## 🔹 Loops

```js
// For loop
for (let i = 0; i < 5; i++) {
  console.log(i);
}

// While loop
let j = 0;
while (j < 5) {
  console.log(j);
  j++;
}

// Do...while
let k = 0;
do {
  console.log(k);
  k++;
} while (k < 5);
```

---

## 🔹 Array Methods

```js
let arr = [1, 2, 3, 4, 5];

// forEach
arr.forEach(num => console.log(num));

// map
let doubled = arr.map(num => num * 2);

// filter
let evens = arr.filter(num => num % 2 === 0);

// find
let firstEven = arr.find(num => num % 2 === 0);
```

---

## 🔹 Functions

```js
// Normal Function
function add(a, b) {
  return a + b;
}

// Arrow Function
let multiply = (a, b) => a * b;

// Function Expression
const square = function(x) {
  return x * x;
};
```

---

## 🔹 Objects

```js
let person = {
  name: "Ali",
  age: 22,
  greet: function() {
    console.log("Hello " + this.name);
  }
};

console.log(person.name); // Ali
person.greet(); // Hello Ali
```

---

## 🔹 ES6+ Features

```js
// Template Literals
let name = "Hasnain";
console.log(`Hello, ${name}!`);

// Destructuring
let user = {id: 1, username: "Ali"};
let {id, username} = user;

// Spread Operator
let arr1 = [1, 2];
let arr2 = [...arr1, 3, 4]; // [1,2,3,4]

// Default Parameters
function greet(msg = "Hello") {
  console.log(msg);
}
```

---

## 📌 Summary

* JavaScript ek **dynamic language** hai.
* Array methods like `map`, `forEach`, `filter` everyday use ke liye important hain.
* ES6 features (`let`, `const`, arrow functions, template literals) modern JS likhne ke liye best hain.

---

✍️ Author: *Hasnain Abbas*
📅 Last Updated: 2025
