# ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run

**EXECUT.ION CONTEXTS**
The JavaScript interpreter uses the concept of execution contexts. 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope.

## EXECUTION CONTEXT & HOISTING
**Each time a script enters a new execution context, there are two phases of activity:** 
 1. PREPARE 

 -  The new scope is created 
 -  Variables, functions, and arguments are created 
  - The value of the this keyword is determined

2. EXECUTE
- Now it can assign values to variables 
- Reference functions and run their code 
- Execute statements 

*UNDERSTANDING SCOPE*
In the interpreter, each execution context has its own va ri ables object. 
It holds the variables, functions, and parameters available within it. 
Each execution context can also access its parent's v a ri ables object.

![scope](https://miro.medium.com/max/4676/1*yGfmo21OoOTPAg0KAxU5GA.png)

**UNDERSTANDING ERRORS**
If a JavaScript statement generates an error, then it throws an **exception.** 
At that point, the interpreter stops and looks for exception-handl ing code.

#### ERROR OBJECTS
Error objects can help you find where your mistakes are 
and browsers have tools to help you read them. 

**ERROR OBJECTS CONTI NUED**
1. Syntax Error 
2. Ref erenceError 
3. Ev alError 
4. UR I Error 

**HOW TO DEAL WITH ERRORS**
Now that you know what an error is and how the browser treats them, 
there are two things you can do with the errors. 

1.  DEBUG THE SCRIPT TO FIX ERRORS
2. HANDLE ERRORS GRACEFULLY 

**HANDLING EXCEPTIONS**
If you know your code might fail, use try, catch, and finally. 
Each one is given its own code block.
1. TRY 
First, you specify the code 
that you think might throw an 
exception within the try block. 

2. CATCH 
If the try code block throws an 
exception, catch steps in with an 
alternative set of code. 

3. FI NALLY 
The contents of the fi na 11 y 
code block will run either 
way - whether the try block 
succeeded or failed. 

**JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error**

 **The console helps narrow down the area in which the error is located, so you can try to find the exact error.**
 **Debugging is the process of finding errors. It involves a process of deduction.**
 