# ProgrammingWithJavaScript

## Functions

### What is a function?

Most of the time you will notice that you need to execute the same set of statements at different points during your program's execution, or in other words, you will notice that you need to combine or bundle a specific functionality and wrap it up or save it in some kind of structure so that you can easily use it when needed. Functions allow you to do exactly that, they are a special block of code that performs a certian functionality the same way every time they get called.

In Javascript, the general syntax for writing functions is as follows:

`function functionName(argumnt/s) {`

  `return value;`

`}`

Functions usually perfrom a set of instructions on the parameters that are passed as arguments when the function gets called, then if the return statement is included, the function will return a value depending on the arguments passed and the body of the function itself.

If the parameters are primitive values, they get passed by value, meaning that the function makes use of thier values but they do not get changed or modified unless they are defined as global variables, also, if parameters are some kind of data sructures, they get passed by reference, meaning that any change on thier value will refelct on any other variable having the same reference to that value unless we clone that value.

### Functions as expressions

As discussed before, when a function contains a return statement, they function call can be used as an expression, meaning that it will return a value, and we can operate on that value. To call a function, you can just type its name followed by a pair of paranthesies holding the arguments for the function, so for example:

`addNumbers(arg1, arg2);`

### Functions and scopes

In general, defining a function the same way explained above will make the function available to the whole code, meaning that it can get called from anywhere inside your code, however, if you use the other ways to define functions ans assign then to variables, you will have to define or decalre that function above any line of code that might need to call this function or you might get an error.

`let myFunc = function func(x,y) {`

  `return x + y`

`}`

### The stack

In simple terms, the stack acts like a vertual table that holds the order all functionsin your code are being executed. 

### Recursion 

Recursion stands for the action of a function calling itself, and usually this behaviour is defined inside the body of the function. Care need to be taken though, since misusing recursion may overflow the stack and make your machine run out of memory.

### Closure

Closure means that nested functions, or functions that are defined inside other functions will have full access to the variables defined inside the outer function, however, the outer function does not have the same functionaity.






