# **Taking Decisions: if/else Statements**

if/else statements in JavaScript allow us to perform conditional execution of code based on a specified condition. The basic structure of an if/else statement is as follows:
```
if (condition) {
  // Code to be executed if the condition is true
} else {
  // Code to be executed if the condition is false
}
```

Here's an explanation of each part of the if/else statement:

* **condition:** This is the expression that is evaluated to determine if it's true or false. If the condition evaluates to true, the code block inside the if statement is executed. Otherwise, the code block inside the else statement (if present) is executed.

* **Code to be executed:** This is the block of code that gets executed if the condition is true (inside the if block) or false (inside the else block).

**Example 1: Checking a Condition**

Let's say we have a variable age representing a person's age, and we want to check if the person is old enough to vote (age >= 18). If they are old enough, we'll display a message saying they can vote. Otherwise, we'll display a message saying they are not old enough. Here's how we can do it with an if/else statement:
```
let age = 20;

if (age >= 18) {
  console.log("You are old enough to vote.");
} else {
  console.log("You are not old enough to vote.");
}
```
In this example, if the age is 20, the condition age >= 18 evaluates to true, so the code block inside the if statement is executed, and the message "You are old enough to vote." is printed to the console.

**Example 2: Checking Multiple Conditions**

We can also use if/else statements to check multiple conditions using `else if`. Let's consider a grading system where we have different ranges for different grades. We'll check the score and assign a grade based on the range. Here's an example:
```
let score = 85;
let grade;

if (score >= 90) {
  grade = "A";
} else if (score >= 80) {
  grade = "B";
} else if (score >= 70) {
  grade = "C";
} else if (score >= 60) {
  grade = "D";
} else {
  grade = "F";
}

console.log("Your grade is " + grade);
```

In this example, the score is `85`. The if/else statement checks the score against multiple conditions. Since `85` is greater than or equal to `80`, the condition score `>= 80` evaluates to true. Therefore, the code block inside the corresponding else if statement is executed, and the grade variable is assigned the value `"B"`. Finally, the grade `"B"` is printed to the console.

That's a brief explanation of `if/else` statements in JavaScript. They allow us to control the flow of our code based on specified conditions, enabling different paths of execution depending on whether the condition is true or false.
