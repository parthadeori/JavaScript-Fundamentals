# **Data Types in JavaScript**

JavaScript is a dynamically typed language, which means variables can hold values of different types. In this guide, we will explore the various data types in JavaScript and provide examples for each.

## **Primitive Data Types**

JavaScript has six primitive data types:

**1. Number**

The number data type represents numeric values, including integers and floating-point numbers.

*Example:*
```
let age = 25;
let pi = 3.14159;
```

**2. String**

The string data type represents a sequence of characters, enclosed in single ('') or double ("") quotes.

*Example:*
```
let name = "John Doe";
let message = 'Hello, World!';
```

**3. Boolean**

The boolean data type represents a logical value of either true or false.

*Example:*
```
let isLogged = true;
let hasPermission = false;
```

**4. Null**

The null data type represents the intentional absence of any object value.

*Example:*
```
let person = null;
```

**5. Undefined**

The undefined data type is used when a variable has been declared but has not been assigned a value.

*Example:*
```
let email;
console.log(email); // Output: undefined
```

**6. Symbol (added in ES6)**

The symbol data type represents a unique and immutable value that can be used as an identifier for object properties.

*Example:*
```
const id = Symbol('id');
let user = {
  name: 'John',
  [id]: 123
};
```

## **Complex Data Types**

JavaScript also has two complex data types:

**1. Object**

The object data type represents a collection of key-value pairs and can hold any type of value.

*Example:*
```
let person = {
  name: 'John Doe',
  age: 25,
  city: 'New York'
};
```

**2. Array**

The array data type represents an ordered collection of values, which can be of any type.

*Example:*
```
let numbers = [1, 2, 3, 4, 5];
let fruits = ['apple', 'banana', 'orange'];
```

## **Checking Data Types**

To check the data type of a value or variable, you can use the typeof operator.

*Example:*
```
let age = 25;
console.log(typeof age); // Output: "number"

let name = "John Doe";
console.log(typeof name); // Output: "string"

let isLogged = true;
console.log(typeof isLogged); // Output: "boolean"

let person = { name: 'John', age: 25 };
console.log(typeof person); // Output: "object"

let numbers = [1, 2, 3, 4, 5];
console.log(typeof numbers); // Output: "object"
```

Understanding the different data types in JavaScript is crucial for working with variables and manipulating data. By leveraging these data types effectively, we can create powerful and dynamic applications.
