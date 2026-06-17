# conditional-statements-questions
"Add 50 conditional statements Q&As".

Part 1: Basic Conditional Concepts
### 1. What is a conditional statement in programming?    

A conditional statement is a control structure that allows a program to execute different blocks of code depending on whether a specified condition evaluates to true or false.

### 2. What does an if statement do?    

An if statement evaluates a condition. If the condition is true, it executes the block of code immediately following it; if it is false, the block is skipped.

### 3. What is the purpose of an else block?    

The purpose of an else block is to provide an alternative path of execution. It defines a block of code that runs only when the corresponding if condition evaluates to false.

### 4. When is an else block executed?    

An else block is executed only when all preceding conditions in the if (or else if) chain evaluate to false.

### 5. What is a Boolean expression?    

A Boolean expression is an expression that evaluates to one of two possible values: true (usually represented as 1 or non-zero in C/C++) or false (represented as 0).

### 6. Write the syntax of a simple if statement
if (condition) {
    // Code to execute if condition is true
   }

### 7. What operator is commonly used to test equality?
 The double equal sign operator (==) is used to test for equality.

### 8. What does the modulus (%) operator return?.

The modulus (%) operator returns the remainder of the integer division between two numbers.

### 9. How can you check if a number is even?
A number is even if it leaves a remainder of 0 when divided by 2
Condition: number % 2 == 0

### 10. How can you check if a number is odd?
A number is odd if it leaves a remainder of 1 (or a non-zero value) when divided by 2.Condition: number % 2 != 0 (or number % 2 == 1)



Part 2: Advanced Conditionals & Relational Operators

### 11. What is the purpose of else-if?
The else if statement allows you to check multiple sequential conditions. If the initial if statement is false, the program moves on to evaluate the else if condition

### 12. What is a nested if statement? 
A nested if statement is an if statement that is placed inside the body of another if or else block.

### 13. Can an if statement exist without an else?
Yes. An if statement does not require an else block. If the condition is false, the program simply proceeds to the next line of code outside the if structure.

### 14. What is the output when a false condition is tested in an if statement without else?
There is no specific output or action taken. The code block inside the `if` statement is skipped entirely, and execution continues normally with the code that follows.

### 15. What is the role of braces {} in C/C++ conditionals?
Braces `{}` define a block of code. They group multiple statements together so that they all execute as a single unit when a condition is met. *(Note: If braces are omitted, only the single immediate next line belongs to the conditional statement).*

### 16. What does > mean?
The **Greater Than** relational operator. It evaluates to `true` if the value on the left is strictly larger than the value on the right.

### 17. What does < mean?
The **Less Than** relational operator. It evaluates to `true` if the value on the left is strictly smaller than the value on the right.

### 18. What does >= mean?
The **Greater Than or Equal To** relational operator. It evaluates to `true` if the value on the left is either larger than or exactly equal to the value on the right.

### 19. What does <= mean?
The **Less Than or Equal To** relational operator. It evaluates to `true` if the value on the left is either smaller than or exactly equal to the value on the right.

### 20. What does != mean?
The **Not Equal To** inequality operator. It evaluates to `true` if the value on the left is different from the value on the right.

---

## Part 3: Switch Case Statements

### 21. What is a switch statement?
A `switch` statement is a multi-way branch statement that provides an elegant alternative to long `if-else-if` ladders. It tests an expression against a list of constant values (integers or characters).

### 22. What is a case label in a switch statement?
A `case` label represents a specific constant value being compared against the switch expression. If the expression matches the case value, execution begins from that point.

### 23. Why is break used in switch?
The `break` statement is used to terminate a case block. It forces the program to exit the `switch` structure immediately, preventing execution from continuing into subsequent cases.

### 24. What happens if break is omitted?
If a `break` is omitted, execution "falls through" to the next `case` block sequentially, running its code regardless of whether the case matches or not, until a `break` or the end of the switch is reached.

### 25. What is the default case in switch?
The `default` case is an optional block that executes if none of the explicit `case` constants match the switch expression. It acts similarly to the final `else` in an `if-else` chain.

### 26. Can switch compare strings in C++?
**No.** In standard C++, a `switch` statement can only evaluate expressions that resolve to integral types (like `int`, `char`, `short`, or `enum`). It cannot directly match string objects or string literals.

### 27. Which statement is better for many constant choices: if-else or switch?
A `switch` statement is generally better. It is cleaner to read, easier to maintain, and can be optimized by compilers using jump tables, making it faster than a long `if-else` chain.

---

## Part 4: Practical Syntax & Coding Logic

### 28. How do you test whether a value is positive?
* **Condition:** `value > 0`

### 29. How do you test whether a value is negative?
* **Condition:** `value < 0`

### 30. How do you test whether a value is zero?
* **Condition:** `value == 0`

### 31. Write a condition to check if age is at least 18.
* **Condition:** `age >= 18`

### 32. Write a condition to check if marks are above 50.
* **Condition:** `marks > 50`

### 33. What is decision making in programming?
Decision making is the process of evaluating conditional statements during execution to determine the dynamic path or order in which statements are processed based on changing data values.

### 34. Can nested if statements have multiple levels?
**Yes.** You can nest `if` statements as deeply as required by your business logic, though nesting too deeply can make code harder to read and maintain.

---

## Part 5: Logical Operators & Practical Problems

### 35. What is logical AND (&&)?
A logical operator that combines two expressions. It evaluates to `true` **only if both** expressions are true. If the first expression is false, the second is not evaluated (short-circuit evaluation).

### 36. What is logical OR (||)?
A logical operator that combines two expressions. It evaluates to `true` if **at least one** of the expressions is true. It evaluates to `false` only if both are false.

### 37. What is logical NOT (!)?
A unary operator that reverses the logical state of its operand. If a condition is true, `!` makes it `false`, and vice-versa.

### 38. How do you check if a year is divisible by 4?
* **Condition:** `year % 4 == 0`

### 39. What is a leap year?
A leap year is a calendar year containing an extra day (February 29th) added to keep the calendar year synchronized with the astronomical year.

### 40. What is the first condition for a leap year?
The basic condition is that a year must be perfectly divisible by `4`. However, if it is a century year (ends in `00`), it must also be divisible by `400`.
* **Complete logic:** `(year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)`

## 41. How do you find the largest of three numbers?

if (a >= b && a >= c) {
    largest = a;
} else if (b >= a && b >= c) {
    largest = b;
} else {
    largest = c;
}

### 42. How do you find the largest of two numbers?

if (num1 > num2) {
    largest = num1;
} else {
    largest = num2;
}

43. What is an if-else-if ladder?
An if-else-if ladder is a multi-path decision structure where multiple conditions are evaluated sequentially from top to bottom. The first condition that returns true gets its block executed, and the rest of the ladder is skipped.

44. What is the difference between if and switch?
-> if statement: Can evaluate complex logic, ranges, and relational expressions (<, >, &&, ||) working with any data type.

-> switch statement: Only tests a single expression for equality against distinct constant values of integral types (integers or characters).

45. Can switch use ranges directly?
No. Standard C/C++ switch syntax requires specific constant values for individual case labels.

46. What is fall-through in switch?
Fall-through is a behavior in a switch statement where a program executes a matching case block and then continues executing subsequent case blocks automatically because a break statement was missing.

47. What data type is usually used for conditions?
The bool (Boolean) data type is used, which stores either true or false.

48. Why are conditional statements important?
Without conditional statements, programs would run linearly, executing the exact same instructions every time. Conditionals give software the ability to adapt, react to different inputs, make complex decisions, and execute intelligent logic pathing.

49. Give one real-life example of a conditional statement.
An ATM withdrawal sequence: IF the account balance is greater than or equal to the requested withdrawal amount, THEN dispense the cash; ELSE, display an "insufficient funds" error notification.

50. Name four conditional structures covered.    

->Simple if statement    
->if-else statement    
->if-else-if ladder    
->switch-case statement
