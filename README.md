
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


<---------javascript---->     Day:01

Javascript is a cross platform  that are used to make webpages interactive(e.g. having complex animation, clickable buttons, popup menus, etc.). There are also more advanced server side versions of JavaScript such as Node.js, which allow you to add more functionality to a website than downloading files (such as realtime collaboration between multiple computers).
     
 cross platform  means Operating Systems:
JavaScript can execute on different operating systems such as Windows, macOS, Linux, Android, and iOS.

3. JavaScript Browser me Kaise Run Hoti Hai?

Browser ke andar ek engine hota hai (Google Chrome me → V8 engine) jo JS code ko samajhta aur execute karta hai.

there are two type of datatype in js
1) premetive data type :-    In JavaScript, primitive data types represent simple, single values that are not objects and have no methods or properties. They are immutable, meaning their values cannot be changed after creation.


1)String, 2)Number, 3)BigInt, 4)Boolean, 5)undifine, 6)Null, 7)symbol
let name = "ali";
name[0]="a";
console.log(name)//output ali // immutable not change
-------------------------------------------------------------------------
arithmetic operator:-
An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value. The standard arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/)
let a = 10, b = 3;
console.log(a + b); // 13
console.log(a - b); // 7
console.log(a * b); // 30
console.log(a / b); // 3.333...
console.log(a % b); // 1
console.log(a ** b);
--------------------------------------------
Assignment Operators (Value dena)
👉 Ye variable ko value assign karte hain.
Operator	Meaning	       Example	        Same As
=	Assign value	        x = 5	        x = 5
+=	Add and assign   	x += 2    	x = x + 2
-=	Subtract and assign	x -= 2	        x = x - 2
*=	Multiply and assign	x *= 2   	x = x * 2
/=	Divide and assign	x /= 2   	x = x / 2
%=	Modulus and assign	x %= 2	        x = x % 2
Example Code:
let x = 10;
x += 5; // 15
x -= 3; // 12
x *= 2; // 24
x /= 4; /
----------------------------------------------
Comparison Operators (Tula karna)
👉 Ye values ko compare karte hain aur true ya false return karte hain.
Operator	Meaning 	                   Example                 Result
==	Equal (sirf value check karega) 	    5 == "5"	           true
===	Strict equal (value + type dono check)	    5 === "5"	           false
!=	Not equal (sirf value check)	            5 != "5" 	           false
!==	Strict not equal (value + type dono check)     5 !== "5"	   true
>	Greater than		                      10 > 5               true  
<	Less than	                               10 < 5          	  false
>=	Greater or equal		                5 >= 5             true
<=	Less or equal		                        5 <= 3                   false

👉 Example Code:
console.log(5 == "5");   // true
console.log(5 === "5");  // false
console.log(5 != "5");   // false
console.log(5 !== "5");  // true
console.log(10 > 3);     // true
console.log(10 < 3);     // false
--------------------------------
Logical Operators (Condition check karna)
👉 Ye mostly if conditions me use hote hain.

Operator	Meaning	                             Example	                                      Result
&&	AND (dono condition true honi chahiye)	     (5 > 3 && 10 > 5)	  true
`		`	OR (ek condition bhi true ho to chalega)
!	NOT (ulta kar deta hai)	                    !(5 > 3)	                        false
👉 Example Code:
let a = 10, b = 20;
console.log(a > 5 && b > 15); // true (dono true)
console.log(a > 15 || b > 15); // true (ek true hai)
console.log(!(a > 5));         // false (ulta kar diya)
=======================================================================================================================================================================
                                                   Day:02                            date:8/26/2025
Switch Statement: 
switch statement is used to perform different action based on different condition.
or
use the switch statement to select one or more block of code to be executed.
Definition

Switch statement ek aisi control statement hai jo multiple conditions ko handle karne ke liye use hoti hai.
def;---
Ye ek value ko different cases ke sath match karti hai aur jis case me match ho, uska code run hota hai.

 Simple def:
Agar aapke paas if-else ladder hai (bohot sari conditions), to uska short aur clean version switch hota hai.
switch(expression) {
  case value1:
    // agar expression == value1
    break;

  case value2:
    // agar expression == value2
    break;

  default:
    // agar koi bhi case match na ho
}
example:   
let day = 3;

switch(day) {
  case1:  //agr case ur number k darmiyan space dana zarori h wrna syntax error ayaga
case 1:
    console.log("Monday");
    break;

  case 2:
    console.log("Tuesday");
    break;

  case 3:
    console.log("Wednesday");
    break;

  case 4:
    console.log("Thursday");
    break;

  case 5:
    console.log("Friday");
    break;

  case 6:
    console.log("Saturday");
    break;

  case 7:
    console.log("Sunday");
    break;

  default:
    console.log("Invalid Day!");
}
========================================================================
Prompt:-The prompt box allows you to ask the user for input. It provides a text field where the user can enter data and a OK and Cancel button.
--> You can use this to collect information from the user,
 like their name, age, or email.
example
let num = parseIntprompt("Enter a number")
console.log((num))

 Alert :-
It is used to display a message to the user, typically for informational purposes.

Assignment01
Instructor : Muhammad Kashan

Q1. Write a program to create a calculator for +,-,*, / & % using if
statements. Take the following input from user through prompt:
a. First number
b. Second number
c. Operation (+, -, *, /, %)
Compute & show the calculated result to user in alert.
======================
let firstNumber = Number(prompt("enter your num"));
// console.log(firstNumber);
let secondNumber = parseInt(prompt("enter your second num"));
// console.log(secondNumber)
let operation = prompt("+, -, *, /, %")
if(operation === "+"){
  alert(firstNumber + secondNumber);
}
else if(operation === "-"){
  alert(firstNumber - secondNumber);
}
else if (operation === "*"){
  alert(firstNumber * secondNumber);
}
else if(operation === "/"){
  alert(firstNumber / secondNumber);
}
else if(operation === "%"){
  alert(firstNumber / secondNumber);
}
else{
  alert("please enter your valid number")
}
Q2. Write a program that takes input a number from user & state whether
the number is positive, negative or zero.
sol:-
let number = parseInt(prompt("enter your number"));
// console.log(number)
if(number > 0){
  alert("result postive")
}
else if (number < 0){
  alert("result negative")
}
else if (number === 0){
  alert("result zero")
}
else{
  alert("please enter your valid number")
}
=========================================================================
1)if Statement:-
👉 Matlab: agar (if) condition true hai to code chalao.
2) else Statement
👉 Matlab: agar if wali condition false ho jaye to else ka code chalao.
3) else if Statement:-
👉 Matlab: agar pehli condition false ho jaye to doosri condition check karo.
eg:
let num = 25;
if(num>18&&num===25){
  console.log("you are eliglbe in id card")
}
else{
console.log("you are not eligble for the id card")
}
example:
let age = 15;

if (age >= 18) {
  console.log("You are adult");
} else {
  console.log("You are minor");
}
===========================================================================
   q1           date27/8/2025             day:03
non premitive datatype:
array and array method:
============================================================================
       day:04
 loop , while loopand do while loop
loop exapmle:
let arr = ["red", "blue", "green", "white", "black"];
let newArr = [];
for(let i=0; i<arr.length; i++){
 newArr.push(arr[i]);
}
 console.log(newArr)


JavaScript mein "iterating" ka matlab hota hai kisi cheez (jaise array, object, string) ke elements ko ek ek karke access karna aur un par koi action perform karna.
1. forEach() kya hai?

forEach() ek array method hai JavaScript mein, jo array ke har element par ek function run karta hai.
Matlab: har element ko ek ek karke iterate karega aur jo kaam aap function mein likhoge wo us element par perform karega.

👉 Ye sirf arrays ke liye kaam karta hai (objects ya strings ke liye directly nahi).

🔹 2. Basic Syntax
array.forEach(function(element, index, array) {
  // yahan aap code likhoge
});


element → current value (jo abhi array ke andar hai)

index → current value ka index (position)

array → pura array jisme loop chal raha hai

🔹 3. Example: Simple Use
let numbers = [10, 20, 30];

numbers.forEach(function(num) {
  console.log(num);
});


👉 Output:

10
20
30


Yahan har element (10, 20, 30) ko print kiya gaya.

🔹 4. Example: Index bhi use karna
let fruits = ["apple", "banana", "mango"];

fruits.forEach(function(fruit, index) {
  console.log(index + " → " + fruit);
});


👉 Output:

0 → apple
1 → banana
2 → mango

🔹 5. Arrow Function ke sath
let fruits = ["apple", "banana", "mango"];

fruits.forEach((fruit, index) => {
  console.log(`${index}: ${fruit}`);
});

🔹 6. Important Points

forEach() return nahi karta (jaise map() ek naya array return karta hai, lekin forEach() kuch return nahi karta).

Iska use tab hota hai jab aapko sirf array ke har element par koi kaam karna ho (e.g., print karna, sum nikalna, ya database mein bhejna).

Ye sirf arrays ke sath hi kaam karta hai.

🔹 7. Example: Sum calculate karna
let numbers = [1, 2, 3, 4, 5];
let sum = 0;

numbers.forEach(function(num) {
  sum += num;
});

console.log("Sum = " + sum);


👉 Output:

Sum = 15
⚡ Summary:
forEach() ek array method hai jo har element ko ek ek karke iterate karta hai aur us par function apply karta hai.
Ye mostly tab use hota hai jab aapko sirf action perform karna ho, new array create nahi karna.
=====================
numbers = [1, 2, 3, 4, 5]
sum = 0
Pehla element (num = 1)


sum = sum + num
sum = 0 + 1
sum = 1
Dusra element (num = 2)


sum = 1 + 2
sum = 3
Teesra element (num = 3)


sum = 3 + 3
sum = 6
Chautha element (num = 4)


sum = 6 + 4
sum = 10
Paanchwa element (num = 5)


sum = 10 + 5
sum = 15
===================================================================
1. map() kya hai?

map() bhi ek array method hai JavaScript mein, lekin iska kaam thoda alag hai:

map() har element par function apply karta hai

Aur ek naya array return karta hai (jo transformed values rakhta hai).

👉 Matlab: Purana array safe rehta hai, aur ek naya array ban jata hai jis mein function ka result hota hai.

🔹 2. Syntax
let newArray = array.map(function(element, index, array) {
  // yahan return karo jo naya value banana ho
});


element → current value (jo abhi array mein hai)

index → current value ka index

array → pura array

🔹 3. Example: Double numbers
let numbers = [1, 2, 3, 4, 5];

let doubled = numbers.map(function(num) {
  return num * 2;
});

console.log(doubled);


👉 Output:

[2, 4, 6, 8, 10]


⚡ Notice: Purana array [1,2,3,4,5] same hi hai, naya array doubled bana.

🔹 4. Example: Arrow function ke sath
let numbers = [10, 20, 30];

let half = numbers.map(num => num / 2);

console.log(half);


👉 Output:

[5, 10, 15]

🔹 5. Example: Strings modify karna
let fruits = ["apple", "banana", "mango"];

let upperFruits = fruits.map(fruit => fruit.toUpperCase());

console.log(upperFruits);


👉 Output:

["APPLE", "BANANA", "MANGO"]

🔹 6. Important Points

map() hamesha ek naya array return karega (empty array bhi ho sakta hai).

forEach() sirf action karta hai (return kuch nahi).

map() zyada useful hai jab aapko array ke elements ko transform/change karna ho.

🔹 7. forEach() vs map() (difference)
Feature	forEach()	map()
Return value	❌ kuch return nahi karta	✅ ek naya array return karta
Use case	Action perform karna (print, sum, DB save)	Naya array banana (transform karna)
Mutate array?	❌ Purana array same rehta hai	❌ Purana array same rehta hai
Example output	undefined	[transformed values]

⚡ Summary:

forEach() = sirf kaam karo (action)

map() = har element ko change karke naya array banao
==================================
🔹 Transform ka matlab

Kisi value ko change karna / nayi shape mein le aana.
Original array ka element ek form mein hota hai, aur map() usse dusri form mein convert karke naya array banata hai.

Array ke elements ko ek nayi form (shape) mein badal kar ek naya array banana.
=========================================
🔹 1. Arrow Function kya hai?

Arrow function JavaScript ka ek short aur modern way hai function likhne ka.
Ye ES6 (2015) mein introduce hua tha.

👉 Matlab: Normal function likhne ke bajaye, ek chhota aur simple syntax mil jata hai.

🔹 2. Syntax
Normal Function:
function add(a, b) {
  return a + b;
}

Arrow Function:
let add = (a, b) => {
  return a + b;
};


👉 Dono same kaam karte hain, bas likhne ka style alag hai.

🔹 3. Short Form (single line return)

Agar function ke andar sirf ek hi statement return karni ho, to {} aur return bhi chhod sakte ho:

let add = (a, b) => a + b;

console.log(add(5, 3)); // 8

🔹 4. Agar parameter ek ho

Agar function mein sirf ek parameter ho, to () bhi optional hai:

let square = x => x * x;

console.log(square(4)); // 16

🔹 5. Agar parameter na ho

Agar function mein koi parameter nahi hai, to () likhna zaroori hai:

let sayHello = () => console.log("Hello World!");

sayHello();

🔹 6. Arrow function aur this

Ye thoda important hai 🔑:

Normal function ke andar this apni khud ki value rakhta hai.

Lekin arrow function apna this create nahi karta, wo outer function ka this use karta hai.

Example:
function normalFunc() {
  console.log(this); 
}

let arrowFunc = () => {
  console.log(this);
}

normalFunc();  // apna `this` dikhayega (browser mein Window object)
arrowFunc();   // outer scope ka `this` lega

🔹 7. Real-life Example with Array
let numbers = [1, 2, 3, 4];

let doubled = numbers.map(num => num * 2);

console.log(doubled); // [2, 4, 6, 8]


👉 Yahaan arrow function ko use karke code chhota aur readable ho gaya.

🔹 8. Kab use karna chahiye?

Jab chhoti aur simple function likhna ho.

Jab array methods (map, filter, forEach, reduce) ke andar function pass karna ho.

Jab apko this ka context outer scope ka chahiye.

✅ Summary:

Arrow function = ek modern aur short way functions likhne ka.

function keyword ki jagah => ka use hota hai.

Chhoti lines mein function likhne ke liye best hai.

Apna this nahi banata (outer this use karta hai).
