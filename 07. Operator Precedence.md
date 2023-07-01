# **Operator Precedence in JavaScript**

Operator precedence determines the order in which operators are evaluated in an expression. JavaScript follows a set of rules to determine the precedence of operators. This guide explains operator precedence in JavaScript, provides code examples, and suggests websites for further help.

## **Understanding Operator Precedence**

JavaScript uses a combination of arithmetic, comparison, logical, and other operators. When multiple operators are present in an expression, JavaScript evaluates them based on their precedence level. Operators with higher precedence are evaluated first.

*For example:*
```
let result = 2 + 3 * 4;
```

In this expression, the multiplication (*) operator has higher precedence than the addition (+) operator. So, 3 * 4 is evaluated first, resulting in 12. Then, the addition operation is performed as 2 + 12, resulting in 14.

## **Operator Precedence Table**

Here is a simplified operator precedence table in JavaScript, from highest to lowest precedence:

* **Grouping:** ()
* **Member Access:** .
* **Computed Member Access:** []
* **Function Call:** ()
* **Postfix Increment/Decrement:** ++, --
* **Unary Operators:** +, -, !, typeof, void, delete, await
* **Exponentiation:** **
* **Multiplication, Division, Remainder:** *, /, %
* **Addition, Subtraction:** +, -
* **Bitwise Shift:** <<, >>, >>>
* **Relational:** <, >, <=, >=, instanceof, in
* **Equality:** ==, !=, ===, !==
* **Bitwise AND:** &
* **Bitwise XOR:** ^
* **Bitwise OR:** |
* **Logical AND:** &&
* **Logical OR:** ||
* **Conditional (Ternary):** ? :
* **Assignment:** =, +=, -=, *=, /=, %=, <<=, >>=, >>>=, &=, ^=, |=, **=

## **Managing Precedence with Parentheses**

Parentheses can be used to override the default operator precedence and explicitly define the order of evaluation.
```
let result = (2 + 3) * 4;

console.log(result); // Output: 20
```

In this example, (2 + 3) is evaluated first, resulting in 5. Then, 5 * 4 is evaluated, resulting in 20.

## **Resources for Further Help**

If you want to explore operator precedence in more detail or need assistance with complex expressions, these websites provide helpful resources:

* **[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_precedence)**
* **[W3Schools JavaScript Operators](https://www.w3schools.com/js/js_precedence.asp)**

These resources offer comprehensive explanations, examples, and tables to understand operator precedence in JavaScript effectively.

Understanding operator precedence is crucial for writing correct and predictable JavaScript code. By following the rules of operator precedence and utilizing parentheses when needed, we can ensure that your expressions are evaluated in the desired order.
