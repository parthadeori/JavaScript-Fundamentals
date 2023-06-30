# **Function Declarations vs. Function Expressions in JavaScript**

In JavaScript, there are two common ways to define functions: `function declarations` and `function expressions`. While they both allow us to create reusable blocks of code, there are some key differences in their syntax and behavior.

## **Function Declarations**

A `function declaration` is a statement that defines a named function using the `function` keyword. It has the following syntax:

```javascript
function functionName(parameters) {
  // Function body - code to be executed
}
```

Here's an example of a function declaration:

```javascript
function greet(name) {
  console.log('Hello, ' + name + '!');
}

greet('John'); // Output: Hello, John!
```

In this example, we define a function called `greet` using a function declaration. It takes a parameter `name` and logs a greeting message to the console. We then call the function `greet` with the argument `'John'`, resulting in the output `Hello, John!`.

`Function declarations` are hoisted in JavaScript, which means they are available for use before they are declared in the code. This allow us to call a function declaration even before its actual declaration in the code.

## **Function Expressions**

A `function expression` is an assignment of a function to a variable or a constant. It has the following syntax:

```javascript
const functionName = function(parameters) {
  // Function body - code to be executed
};
```

Here's an example of a function expression:

```javascript
const greet = function(name) {
  console.log('Hello, ' + name + '!');
};

greet('John'); // Output: Hello, John!
```

In this example, we define a function expression by assigning an anonymous function to the `greet` constant. It takes a parameter `name` and logs a greeting message to the console. We then call the function `greet` with the argument `'John'`, resulting in the output `Hello, John!`.

Unlike `function declarations`, `function expressions` are not hoisted. They must be defined before they are called in the code. Since function expressions are assigned to variables, the variable name can be used to invoke the function.

## **Key Differences**

Here are some key differences between `function declarations` and `function expressions`:

- **Hoisting**: `Function declarations` are hoisted, meaning they can be called before their actual declaration in the code. `Function expressions` are not hoisted and must be defined before they are used.

- **Naming**: `Function declarations` have a mandatory name, which is used to call the function. `Function expressions` can be named or anonymous, depending on whether a name is assigned to the variable or constant.

- **Flexibility**: `Function expressions` offer more flexibility than `function declarations`. They can be assigned to variables, passed as arguments to other functions, and created dynamically at runtime.

- **Scope**: Both `function declarations` and `function expressions` create functions within the current scope. However, since `function expressions` are assigned to variables, they have the added benefit of being able to close over variables from their containing scope.

---

`Function declarations` and `function expressions` are both powerful ways to define functions in JavaScript. Understanding their differences and appropriate use cases will help us write clean and efficient code.
