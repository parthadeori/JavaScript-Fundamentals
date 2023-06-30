# Logical Operators in JavaScript

Logical operators in JavaScript are used to combine or manipulate boolean values. JavaScript provides three main logical operators: AND (`&&`), OR (`||`), and NOT (`!`).

## AND Operator (`&&`)

The AND operator (`&&`) returns `true` if both operands are `true`. Otherwise, it returns `false`. It evaluates the second operand only if the first operand is `true`.

```javascript
console.log(true && true);   // true
console.log(true && false);  // false
console.log(false && true);  // false
console.log(false && false); // false
```

In the above example, the AND operator combines two boolean values using `&&`. The result is `true` only if both operands are `true`.

The AND operator is often used in conditional statements to check multiple conditions at once. If all the conditions are true, the code inside the conditional statement will execute.

```javascript
let age = 25;
let hasLicense = true;

if (age >= 18 && hasLicense) {
  console.log("You can drive.");
} else {
  console.log("You cannot drive.");
}
```

In the above example, the AND operator is used to combine two conditions: `age >= 18` and `hasLicense`. If both conditions are `true`, the message "You can drive." will be displayed. Otherwise, the message "You cannot drive." will be displayed.

## OR Operator (`||`)

The OR operator (`||`) returns `true` if at least one of the operands is `true`. If both operands are `false`, it returns `false`. It evaluates the second operand only if the first operand is `false`.

```javascript
console.log(true || true);   // true
console.log(true || false);  // true
console.log(false || true);  // true
console.log(false || false); // false
```

In the above example, the OR operator combines two boolean values using `||`. The result is `true` if either of the operands is `true`.

The OR operator is useful when you want to execute code if any of the conditions are true.

```javascript
let hour = 10;

if (hour < 6 || hour > 18) {
  console.log("Good evening!");
} else {
  console.log("Good day!");
}
```

In the above example, the OR operator is used to check if `hour` is less than 6 or greater than 18. If either condition is true (i.e., if the hour is before 6 am or after 6 pm), the message "Good evening!" will be displayed. Otherwise, the message "Good day!" will be displayed.

## NOT Operator (`!`)

The NOT operator (`!`) negates the boolean value of its operand. It returns `true` if the operand is `false`, and `false` if the operand is `true`.

```javascript
console.log(!true);  // false
console.log(!false); // true
```

In the above example, the NOT operator negates the boolean values. It flips `true` to `false` and `false` to `true`.

The NOT operator is commonly used to check for the absence of a condition or to toggle a boolean value.

```javascript
let isLoggedIn = false;

if (!isLoggedIn) {
  console.log("Please log in to continue.");
} else {
  console.log("Welcome!");
}
```

In the above example, the NOT operator is used to check if `isLoggedIn` is `false`. If it is `false`, the message "Please log in to continue." will

 be displayed. Otherwise, the message "Welcome!" will be displayed.

## Precedence and Parentheses

When using multiple logical operators in an expression, it's important to understand their precedence. The NOT operator (`!`) has the highest precedence, followed by the AND operator (`&&`), and finally the OR operator (`||`). However, it's a good practice to use parentheses to make the order of evaluation clear and avoid confusion.

```javascript
let result = (true || false) && !true;
console.log(result); // false
```

In the above example, parentheses are used to explicitly group the OR operation first (`true || false`). Then, the NOT operator negates the result (`!true`). Finally, the AND operator combines the two values.

## Conclusion

Logical operators in JavaScript allow you to perform logical operations on boolean values. Understanding how to use the AND (`&&`), OR (`||`), and NOT (`!`) operators is essential for creating conditional logic and controlling the flow of your JavaScript programs.
