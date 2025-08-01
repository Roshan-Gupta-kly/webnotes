# JavaScript
JavaScript is an Object Oriented Programming Languages.
<hr>

## Data Types

**What is a data type, and what are the different data types in JavaScript?**

In JavaScript, a data type refers to the kind of value a variable holds.

A variable is a named container that stores a value of a specific data type, allowing you to reference and manipulate it throughout your code. Data types help the program understand the kind of data it's working with, whether it's a number, text, or something else.

JavaScript has several basic data types that you'll use in your programs. We'll explore each data type in greater detail in future lecture videos. For now, here is a brief introduction of the different data types in JavaScript.

The first data type we will look at is the Number type.

A Number represents both integers and floating-point values. Examples of integers include 7, 19, and 90. Examples of floating point numbers include 3.14 and 5.2. A floating point number is a number with a decimal point.

The next data type is a String.

A ***String*** is a sequence of characters, or text, enclosed in quotes. Here are two examples:

```js
  "Hello, world"
  'JavaScript'
```

Another data type used in JavaScript is the Boolean type.

A ***Boolean*** represents one of two possible values: true or false. You can use a boolean to check if a page is loading, or if a user is logged in or not.

The next two data types used in JavaScript are undefined and null.

***Undefined*** means a variable has been declared but hasn't been given a value yet. ***Null*** means the variable has been intentionally set to "nothing" and does not hold any value. We will explore more on how this works in future lectures.

The next data type we will look at is the Object type.

An ***Object*** is a more complex data type that can hold collections of key-value pairs. Let's break this down. The key (also called a property name), is like a label for the data, whereas the value, is the actual data you want to store. Here is an example:
```js
let book = {
  title: "The Great Gatsby",
  author: "F. Scott Fitzgerald",
  year: 1925
};
```
In this object, title, author, and year are the keys (or property names). The Great Gatsby, F. Scott Fitzgerald, and 1925 are the corresponding values.

Each key-value pair in an object is called a property. So we can say that this book object has three properties. This is just a basic introduction to objects and their properties. In future videos, we'll go deeper into more advanced concepts.

The last two data types are the Symbol and BigInt data types.

A Symbol is a special type of value in JavaScript that is always unique and cannot be changed. It's often used to create unique labels or identifiers for properties:
```js
// Creating two symbols
const symbol1 = Symbol('mySymbol');
const symbol2 = Symbol('mySymbol');
console.log(symbol1 === symbol2); // Outputs: false
```
In this example, we create two symbols with the same description, but they are unique.

***BigInt*** is used for very large numbers that exceed the limit of the Number type:
```js
const bigNumber = 1234567890123456789012345678901234567890n;
console.log(bigNumber);
// Outputs: 1234567890123456789012345678901234567890n
```
In this example, we create a BigInt by adding n at the end of a very large number.

Understanding these data types helps you handle and work with various kinds of data in your programs, as each type has its own characteristics and behaviors.
