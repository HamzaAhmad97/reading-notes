# In memory storage

## The JavaScript Call Stack

1. A *call* is basically an invocation of a function, which happens once that function is on top of the stack regardless of the height of the stack.

2. Since Js is single threaded, we have only one call stack, thus, only one call can happen at a time, when the function is on top of the stack.

3. LIFO, short for (last in first out), basically means that the last function that gets pushed on top of the stack gets called or invoked first, and then it gets removed from the stack first, before any other older functions that are in the stack and are yet to return and get removed.

4. As a simple example of a call stack in js, consider the line of code below:

```
function sum(a,b){
  console.log(a,b);
  return double(a) + b;
}

function double(num) {
  console.log(num);
  return num**2;
}
```

This is how the call stack will look like:
<pre>

                                                      log
                       log                 double    double     double
|     | > | sum  | > | sum  | > | sum | > | sum  | > | sum | > | sum  | > | sum | > |    | > |
</pre>

5. Usually stack overflow happens when the stack keeps growing up and no function returns, so we face the possibility of running out of memory and our app becomes unstable, and among the most common examples are recursion, which means when a function keeps calling itself, and other cases that are similar, take the following for an example:

```
function callTwo(){
  callOne()
}

function callOne() {
  callTwo()
}
```

-----------------------------------

## Error messages in Javascript

1. **Reference error**: An error message that gets shown when something bad happens with references to variables, like when you use a variable that is not yet defined, so the reference is not there, and js just throws an error.
2. **Syntax error**: An error message that gets shown when something bad happens with the syntax of the code, or when the interpreter fails to parse some piece of code because it does not agree with the rules of writing the language, like using double equal signs to assign a value to a variable.
3. **Range error**: An error message that gets shown when something bad happens with ranges like the length or the number of items in an array, for example, if you try to assign the length property of an array or change it, this message will get shown.
4. **Type error**: An error message that gets shown when something bad happens with types, that is, when incompatibility occurs, for example, if you try to use `.reverse()` which is an array method on a string, this error will get thrown.

5. a breakpoint is a place you set on purpose at specific lines of code to help you debug and check the flow of data and the possibility of potential errors, the execution will pause at breakpoints.

6. The word *debugger* is used to introduce breakpoints at some lines of code.
