# **let, const, and var in JavaScript**

In JavaScript, `let`, `const`, and `var` are used to declare variables. This guide explains the differences between these keywords, along with code examples and their corresponding outputs.

## **let**

The `let` keyword declares a *block-scoped* variable that can be reassigned a new value. Variables declared with let are mutable.

```
let age = 25;
age = 30; // Value can be reassigned

console.log(age); // Output: 30
```

## **const**

The `const` keyword declares a *block-scoped* variable that holds a constant value, which cannot be reassigned. Variables declared with const are immutable.

```
const pi = 3.14159;

console.log(pi); // Output: 3.14159
```

## **var**

The `var` keyword declares a *function-scoped* or *globally-scoped* variable. Variables declared with var are *hoisted* to the top of their scope and can be reassigned.

```
var count = 10;

console.log(count); // Output: 10
```

**Scope**

The scope determines the visibility and lifetime of variables.

* **Block Scope**

    `let` and `const` variables are block-scoped, meaning they are limited to the block (within curly braces) where they are declared.
```
{
  let x = 5;
  const y = 10;
  var z = 15;

  console.log(x, y, z); // Output: 5 10 15
}

console.log(x, y, z); // Error: x is not defined, y is not defined, 15
```

* **Function Scope**

    `var` variables are function-scoped, which means they are limited to the function where they are declared.
```
function printNumbers() {
  var num1 = 1;
  let num2 = 2;
  const num3 = 3;

  console.log(num1, num2, num3); // Output: 1 2 3
}

printNumbers();
console.log(num1, num2, num3); // Error: num1 is not defined, num2 is not defined, num3 is not defined
```

* **Hoisting**

    Variables declared with `let` and `const` are not hoisted, whereas variables declared with `var` are hoisted.

```
console.log(name); // Output: undefined
var name = 'John';

console.log(age); // Error: age is not defined
let age = 25;
```

## **Conclusion**

Use `let` when we need to reassign the variable.

Use `const` when we want a variable with a constant value.

Use `var` when we want a function-scoped or globally-scoped variable.

Understanding the differences between `let`, `const`, and `var` is essential for proper variable declaration and scoping in JavaScript. Choose the appropriate keyword based on your requirements to write clean and reliable code.
