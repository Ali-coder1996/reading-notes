# Functions:

>Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.


## Defining functions:
Function declarations:
A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

- The name of the function.

- A list of parameters to the function, enclosed in parentheses and separated by commas.

- The JavaScript statements that define the function, enclosed in curly brackets, {...}.

**For example, the following code defines a simple function named square:**

~~~
function square(number) {
  return number * number;
}
~~~

 The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:
>
~~~
return number * number;
~~~


### Function expressions:

While the function declaration above is syntactically a statement, functions can also be created by a function expression.

Such a function can be anonymous; it does not have to have a name. For example, the function square could have been defined as:
>
~~~
const square = function(number) { return number * number }
var x = square(4) // x gets the value 16
~~~

#### Calling functions:

Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:

>
~~~
square(5);
~~~

The preceding statement calls the function with an argument of 5. The function executes its statements and returns the value 25.

Functions must be in scope when they are called, but the function declaration can be hoisted (appear below the call in the code), as in this example:

>
~~~
console.log(square(5));
/* ... */
function square(n) { return n * n }
~~~