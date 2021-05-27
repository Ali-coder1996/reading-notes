## What you should already know :

**This guide assumes you have the following basic background:**

1. A general understanding of the Internet and the World Wide Web (WWW).

2. Good working knowledge of HyperText Markup Language (HTML).

3. Some programming experience. If you are new to programming, try one of the tutorials linked on the main page about JavaScript.
### What is JavaScript?
**JavaScript is a cross-platform, object-oriented scripting language used to make webpages interactive (e.g., having complex animations, clickable buttons, popup menus, etc.).  There are also more advanced server side versions of JavaScript such as Node.js, which allow you to add more functionality to a website than downloading files (such as realtime collaboration between multiple computers). Inside a host environment (for example, a web browser), JavaScript can be connected to the objects of its environment to provide programmatic control over them.**

#### Grammar and types:
*Comments:*

The syntax of comments is the same as in C++ and in many other languages:
// a one line comment

~~~
/* this is a longer,
 * multi-line comment
 */

/* You can't, however, /* nest comments */ SyntaxError */
~~~
##### Declarations:

JavaScript has three kinds of variable declarations.

>var

Declares a variable, optionally initializing it to a value.

>let

Declares a block-scoped, local variable, optionally initializing it to a value.

>const

Declares a block-scoped, read-only named constant.

###### Control flow:

**The control flow is the order in which the computer executes statements in a script.**

**Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.** 

**For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:**

~~~
if (field==empty) {
    promptUser();
} else {
    submitForm();
}
~~~