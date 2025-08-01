Functions are reusable pieces of code that performs a specific task or calculate a value.Think of functions as a machine that takes some input, does some operations on it, and then produces an output.

Here is an example of declaring a function:
```js
function greet(){
console.log("Hello Roshan👋");
```

In this example, we have declared a function called greet. Inside that function, we have a `console.log` that logs the message `Hello Roshan👋`. If we tried to run this code, we would not see the message appear in the console. This is because we need to call the function.

A function call, or or invocation, is when we actually use or execute the function. To call a function, you will need to reference the function name followed by a set of parentheses:

```js
function greet() {
  console.log("Hello Roshan👋");
}

greet(); // "Hello Roshan👋"
```

Now the message of `Hello Roshan👋` will be logged to the console. But what if we wanted the message to say `Hello Yugal👋` or `Hello Prenisha👋`?

We don't want to write a new function each time we greet a different user. Instead, we can create a reusable function that uses function parameters and arguments.

Parameters act as placeholders for the values that will be passed to the function when it is called. They allow functions to accept input and work with that input. Arguments are the actual values passed to the function when it is called. Here is an updated version of the `greet` function that uses parameters and arguments:

```js
function greet(name) {
  console.log("Hello " + name + "👋");
}

greet("Yugal"); // Hello Yugal👋
greet("Prenisha"); // Hello Prenisha👋
```

The `name` serves as the parameter while the strings `Yugal` and `Prenisha` serve as the arguments. Now we have a reusable function that can be used dozens of times throughout our code with different arguments.

When a function finishes its execution, it will always return a value. By default, the return value will be `undefined`. Here is an example:

```js
function doSomething() {
    console.log("Doing something...");
}

let result = doSomething();
console.log(result); // undefined
```
If you need your function to `return` a specific value, then you will need to use the `return` statement. Here is an example of using a return statement to return the sum of two values:

```js
function calculateSum(num1, num2) {
  return num1 + num2;
}

console.log(calculateSum(3, 4)); // 7
```

Often times you will be using the `return` statement, because you can use that value that was output from the function later on in your code.

So far, we've been working with named functions, but you can also create what's called an anonymous function. An anonymous function is a function without a name that can be assigned to a variable like this:

```js
const sum = function (num1, num2) {
  return num1 + num2;
};

console.log(sum(3, 4)); // 7
```

In this example, we have a `const` variable called `sum` and we are assigning it an anonymous function that returns the sum of `num1` and `num2`. We are then able to call `sum` and pass in the numbers `3` and `4` to get the `result` of `7`.

Functions support default parameters, allowing you to set default values for parameters. These default values are used if the function is called without an argument for that parameter. Here's an example:

```function greetings(name = "Guest") {
  console.log("Hello, " + name + "👋");
}

greetings(); // Hello, Guest👋
greetings("Roshan"); // Hello, Roshan👋
```

In this example, if no `argument` is provided for `name`, it defaults to `Guest`.

In summary, functions allow you to write reusable and organized code. They can take inputs (parameters), perform actions, and return outputs.
