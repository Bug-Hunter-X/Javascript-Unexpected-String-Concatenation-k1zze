# Javascript Unexpected String Concatenation
This repository demonstrates a common yet subtle bug in JavaScript where the '+' operator performs string concatenation instead of throwing a type error when different types are added.  This can lead to unexpected results and difficult-to-debug errors.
The `bug.js` file contains the buggy code, while `bugSolution.js` provides a solution demonstrating type checking.

## Bug
The `foo` function in `bug.js` is intended to add two numbers. However, when a number and a string are passed in, JavaScript silently concatenates them instead of raising an error, producing the result '12' instead of 3. This silent failure is a common source of bugs.