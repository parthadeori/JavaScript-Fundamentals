# **Basic Operators in JavaScript**

Operators in JavaScript are symbols or keywords that perform operations on operands (values or variables). This guide explains the various types of basic operators in JavaScript, along with code examples and their corresponding outputs.

## **Arithmetic Operators**

Arithmetic operators are used to perform mathematical calculations on numeric values.

**Addition (+)**

The addition operator `+` is used to add two values together.
```
let sum = 5 + 3;

console.log(sum); // Output: 8
```

**Subtraction (-)**

The subtraction operator `-` is used to subtract one value from another.
```
let difference = 10 - 3;

console.log(difference); // Output: 7
```

**Multiplication (*)**

The multiplication operator `*` is used to multiply two values.
```
let product = 4 * 6;

console.log(product); // Output: 24
```

**Division (/)**

The division operator `/` is used to divide one value by another.
```
let quotient = 15 / 5;

console.log(quotient); // Output: 3
```

**Modulus (%)**

The modulus operator `%` is used to calculate the remainder of a division operation.
```
let remainder = 17 % 5;

console.log(remainder); // Output: 2
```

**Increment (++) and Decrement (--)**

The increment operator `++` and decrement operator `--` are used to increase or decrease the value of a variable by 1.
```
let count = 5;

count++; // Equivalent to count = count + 1;

console.log(count); // Output: 6

count--; // Equivalent to count = count - 1;

console.log(count); // Output: 5
```

## **Assignment Operators**

Assignment operators are used to assign values to variables.

**Assignment (=)**

The assignment operator `=` is used to assign a value to a variable.
```
let age = 25;

console.log(age); // Output: 25
```

**Compound Assignment (+=, -=, *=, /=, %=)**

Compound assignment operators combine arithmetic operations with assignment.
```
let count = 10;

count += 5; // Equivalent to count = count + 5;

console.log(count); // Output: 15

count *= 2; // Equivalent to count = count * 2;

console.log(count); // Output: 30
```

## **Comparison Operators**

Comparison operators are used to compare values and return a boolean result.

**Equality (==)**

The equality operator `==` checks if two values are equal.
```
let num1 = 5;
let num2 = 8;

console.log(num1 == num2); // Output: false
```

**Inequality (!=)**

The inequality operator `!=` checks if two values are not equal.
```
let num1 = 5;
let num2 = 8;

console.log(num1 != num2); // Output: true
```

**Greater than (>)**

The greater than operator `>` checks if the left operand is greater than the right operand.
```
let num1 = 5;
let num2 = 8;

console.log(num2 > num1); // Output: true
```

**Less than (<)**

The less than operator < checks if the left operand is less than the right operand.
```
let num1 = 5;
let num2 = 8;

console.log(num1 < num2); // Output: true
```

**Greater than or equal to (>=)**

The greater than or equal to operator `>=` checks if the left operand is greater than or equal to the right operand.
```
let num1 = 5;
let num2 = 8;

console.log(num2 >= num1); // Output: true
```

**Less than or equal to (<=)**

The less than or equal to operator `<=` checks if the left operand is less than or equal to the right operand.
```
let num1 = 5;
let num2 = 8;

console.log(num1 <= num2); // Output: true
```

## **Logical Operators**

Logical operators are used to combine and manipulate boolean values.

**Logical AND (&&)**

The logical AND operator `&&` returns true if both operands are true.
```
let x = true;
let y = false;

console.log(x && y); // Output: false
```

**Logical OR (||)**

The logical OR operator `||` returns true if at least one of the operands is true.
```
let x = true;
let y = false;

console.log(x || y); // Output: true
```

**Logical NOT (!)**

The logical NOT operator `!` negates the boolean value of its operand.
```
let x = true;

console.log(!x); // Output: false
```

## **Conclusion**

Understanding basic operators in JavaScript is essential for performing calculations, assigning values, and making logical comparisons. By using these operators effectively, we can manipulate and control the flow of your code.
