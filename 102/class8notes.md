# Class 8 Notes - JS Operators and Loops

[Back to Home](../README.md)

## [Expressions and Operation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

Good stuff in the link (more than I expected).  

At a high level, an expression is a valid unit of code that resolves to a value.  
There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate.  

+ Operators join operands.
+ Precedence of operators determines the order they are applied when evaluating an expression
+ When chaining these expressions without parentheses or other grouping operators like array literals, the assignment expressions are grouped right to left (they are right-associative), but they are evaluated left to right.

Assignment Operator 
+ x &&= y only assigns if the x is truthy

Ternary Operator
+ condition ? val1 : val2
+ If condition is true, the operator has the value of val1. Otherwise it has the value of val2. You can use the conditional operator anywhere you would use a standard operator.

Void Operator
+void (expression)  
+ void expression
+ The void operator specifies an expression to be evaluated without returning a value. expression is a JavaScript expression to evaluate. The parentheses surrounding the expression are optional, but it is good style to use them.

## [Loops and Iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

### For

A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

for ([initialExpression]; [conditionExpression]; [incrementExpression])
  {statement}

### While

A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

while (condition)
  {statement}