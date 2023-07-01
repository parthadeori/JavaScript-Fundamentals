# **Function Calling Other Functions in JavaScript**

In JavaScript, functions can call other functions to perform a series of tasks or to achieve a specific goal. This concept is known as "function composition" and is a fundamental aspect of building modular and reusable code.

## **Calling a Function from Another Function**

To call a function from another function, we simply need to invoke the function using its name followed by parentheses `()`. Here's an example:

```javascript
function greet() {
  console.log('Hello!');
}

function sayHello() {
  console.log('Before the greeting...');
  greet(); // Calling the greet() function
  console.log('After the greeting...');
}

sayHello(); // Calling the sayHello() function
```

In the above example, the `sayHello()` function calls the `greet()` function within its body. When `sayHello()` is invoked, it prints "Before the greeting...", then calls `greet()` which prints "Hello!", and finally prints "After the greeting...".

## **Passing Values between Functions**

Functions can also pass values (arguments) to other functions, allowing for dynamic and flexible behavior. Here's an example:

```javascript
function square(number) {
  return number * number;
}

function calculateArea(length, width) {
  const area = square(length) * square(width);
  return area;
}

const areaOfRectangle = calculateArea(4, 6);
console.log(areaOfRectangle); // Output: 144
```

In the above example, the `calculateArea()` function takes two arguments (`length` and `width`) and calls the `square()` function twice, passing the `length` and `width` values as arguments. The `square()` function squares the given number and returns the result. Finally, `calculateArea()` multiplies the squared values and returns the area of the rectangle.

## **Function Chaining**

Function chaining is a technique where the output of one function call is used as input for the next function call. This approach enables a concise and expressive way of performing multiple operations in sequence. Here's an example:

```javascript
function add(num1) {
  return num1 + 5;
}

function multiply(num2) {
  return num2 * 2;
}

function subtract(num3) {
  return num3 - 1;
}

const result = subtract(multiply(add(3)));
console.log(result); // Output: 15
```

In the above example, the functions `add()`, `multiply()`, and `subtract()` are chained together. The value `3` is passed to `add()`, which adds `5` and returns `8`. The result of `add()` is then passed to `multiply()`, which multiplies it by `2` and returns `16`. Finally, the result of `multiply()` is passed to `subtract()`, which subtracts `1` and returns `15`. The final result is stored in the `result` variable and printed to the console.

## **Conclusion**

Calling functions from other functions allows for code reusability, modularity, and the ability to perform complex operations. By passing values and chaining functions, we can create more sophisticated and flexible code structures in JavaScript.
