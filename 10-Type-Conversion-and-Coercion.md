# **Type Conversion in JavaScript**

Type conversion in JavaScript refers to the process of converting a value from one data type to another. JavaScript provides several built-in methods and operators to perform type conversion.

## **Implicit Type Conversion**

Implicit type conversion, also known as **type coercion**, occurs when JavaScript automatically converts the data type of a value to another data type, usually in an expression involving different data types. Here's an example:

```
let number = 42;
let string = "The answer is " + number;

console.log(string); // Output: "The answer is 42"
```

In this example, the `number` variable is implicitly converted to a string by JavaScript when concatenating it with another string using the `+` operator. The resulting string is `"The answer is 42"`.

## **Explicit Type Conversion**

Explicit type conversion, also known as **type casting**, is when we explicitly convert a value from one data type to another using built-in methods or functions. Here are a few examples of explicit type conversion methods in JavaScript:

* **Number():** Converts a value to a number.

```
let stringNumber = "42";
let convertedNumber = Number(stringNumber);

console.log(convertedNumber); // Output: 42
```

In this example, the string `"42"` is explicitly converted to a number using the `Number()` function.

* **String():** Converts a value to a string.

```
let number = 42;
let convertedString = String(number);

console.log(convertedString); // Output: "42"
```

In this example, the number `42` is explicitly converted to a string using the `String()` function.

* **Boolean():** Converts a value to a boolean.

```
let number = 42;
let convertedBoolean = Boolean(number);

console.log(convertedBoolean); // Output: true
```

In this example, the number `42` is explicitly converted to a boolean using the `Boolean()` function. Any non-zero number is converted to `true`, while `0`, `NaN`, `null`, `undefined`, and `empty strings` are converted to `false`.

# **Type Coercion in JavaScript**

Type coercion is the process of converting one data type to another during a comparison or operation. JavaScript performs **implicit type coercion** in various situations, especially when operators are used with operands of different data types.

```
let sum = 5 + "2";

console.log(sum); // Output: "52"
```

In this example, the number `5` is implicitly coerced to a string, and then concatenated with the string `"2"`. The result is the string `"52"`.

It's important to note that **type coercion** can sometimes lead to unexpected or unintended results, so it's crucial to be aware of how JavaScript handles type coercion.

These are the concepts of **type conversion** and **type coercion** in JavaScript. **Type conversion** involves explicitly converting a value from one data type to another, while **type coercion** involves the automatic conversion of data types during operations or comparisons. Understanding these concepts is essential for correctly manipulating and working with different types of data in JavaScript.
