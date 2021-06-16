# Error handling and debugging

## The stack

You can think of the stack as being a to-do list, but not exactly, in simple terms, when a function for instance is currently being executed, it might need to call or invoke other functions, so what the stack is or what it does is that it adds the new function to be called on top of it, the top of the stack, and  the function waits until it gets executed, and so on until we get back to the other function that called the other function, and the process goes on. Each time an item like a function gets added to on top of the stack, it generates an execution context, which can be though of as being a special environment that holds the values of each objects, variables and function related or regestered with that context.

![stack](https://miro.medium.com/max/1592/0*ryPdDzB_jghiVi2e.png)

## Hoisting

Each time some script enters an execution context, it passes through two phases, the first one which is related to preparing objects and variables and the value of the **this** keyword, the other phase is concerned with execution which itself includes assigning values and referencing functions. This allows us to have something called **hoisting**, so for example, when you call a function on a line before it was defined or initialized, JavaScript will not complain as long as the function and the statement that references or executes it is in the same execution context, and that is because the values of variables and objects get prepared before they get used. Also, each execution context can also access its parent's variables object knowing that each execution context has its own va ri ables object.

![hoisting](https://miro.medium.com/max/1182/1*JfVo7EnZ83pEkfzps63K_Q.png)

## Errors and error objects

When a line of code causes an error, it throws and error, the interpreter stops and starts looking for code that will handle that exception, if it does not find one at the same level, it goes a level up, if it still can't find one, it will move up a level and so on.

Actually, when an error occurs or when an exception is thrown, an error object gets created, and this object holds properties about the source and the nature of error. There are a number of predefined error objects that we usually encounter on a daily basis, like the syntax error object.

## Debugging 

Whene encountering an error, you can handle it using try/ except statements, or you can try to debug your code. Debugging means trying fixing or eliminating a bug or an error, and it simply relies on you narrowing down the possible causes of the probelm, the console and the code editors usually show information about the error such as the line number where it occured, but sometimes this can be misleading, and you might need to enclose or limit yourself to smaller chunks of code and start adding **breakpoints** to pause the execution and check for potintial error source by for example observing or checking the resulting values for the variables at hand.

The other way is somewhat more familiar to us, even for new programmers, since it only relies on using the console and the log to show values for things we want to check, all you need is to know where to put this statement and the statement itself `console.log()`. There are other types of console methods that are used almost for the same purpose but they differ by the nature of the thing they are printing, so for example, the `console.error()` is used to hold errors. There are a lot of ways you can utilize the console like printing in tabular form or grouping messages.

## Handling exceptions

To handle exceptions, which are thrown once an error occurs, you need the try/ catch/ finally statements. Basically, we put the code that has the potential to throw an error in the try statement, if an exception is thrown, the execution moves to the following catch statement, which gets passed an optional error object, and then the code inside it gets executed. The code in "finally" gets executed either way.

![try catch finally](https://toppertips-bx67a.ondigitalocean.app/assets/images/try-catch-finally-block.png)

In addition to all of this, you can create your own errors when you expect something to go wrong, the syntax is as follows:

`throw new error('message');`





