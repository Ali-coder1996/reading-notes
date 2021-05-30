## Loops and iteration:
**Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript.**

**You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop:**

~~~
for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}
~~~

>for statement:

**When a for loop executes, the following occurs:**

1- The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.

2- The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)

3- The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.

4-If present, the update expression incrementExpression is executed.

5- Control returns to Step 2

>>while statement:

A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

~~~
while (condition)
  statement
~~~

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

To execute multiple statements, use a block statement ({ ... }) to group those statements

#### Example 1

The following while loop iterates as long as n is less than 3:
~~~
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
~~~

With each iteration, the loop increments n and adds that value to x. Therefore, x and n take on the following values:

1- After the first pass: n = 1 and x = 1

2- After the second pass: n = 2 and x = 3

3- After the third pass: n = 3 and x = 6

>After completing the third pass, the condition n < 3 is no longer true, so the loop terminates.