# Functional programming, modules and require()

## Functional programming

1. From what I know so far, there are two programming paradigms, objcet oriented functional programming. Before diving into defining functional programming as a mere concept, there are some concepts that we should know about, especially in JavaScript. In js, funcitons are actually objects, and they have thier own properties and methods, like arguments as a property, and call as a method. In js, functions are also considered first-class members, meaning that they can be passed as arguments, and they can also be returned from other functions, thanks to arrow functons and functional expressions for making that much easier, so what we really matters is that functions in js can be used almost everywhere other regular bindings or variables can be used. With functional programming, we follow a wider programming paradigm, called declarative programming, which basically focuses on defining *what* should happen over *how* what should happen. In general, functional programming makes your programs as if we are making computations by passing values into functions and so on.

2. Pure functions are functions that do not cause side effects, what are side effects you ask? well, they are when a function depends on something other than its arguments, like for example logging to the console, or modifying a global variable and so on. Pure functions do not do that, and in addition, they only rely on thier arguments, as they also produce the same functions or values for the same set of arguments. Ah, one more thing, for a function to be pure, it should take at least one parameter, else it will definitely cause some side effects.

3. From point 2, pure functions are useful since they do not change anything inside our program since they do not cause any side effects. In addition to that, since they only rely on thier arguments and they pass the same results for the same set of arguments, they are easier to be tested, they can be thought of as independent sets of code and we can test them independently of the environment. They are also easier to maintain and test for the same reasons.

4. To be immutible is to be unchangeable. What ths refers to in functional programming is the data. As mentioned before, we do not need side effects, and we do not want to modify global variables or even any values passed to our functions, so instead, to achieve immutability, we should always make copies of the data we pass to our funcitons since we pass the reference to those data structures in case they are of reference type. For example, with objects, we can use Object.assign() to copy the content of the passed object to another one that is local to our function.

5. Referential transparency can be understood like this, when we have a pure function, and pass it a value, it will always return the same result, thus we say it is referentially transparent. With this, we can use those functions, especially when they are written as expressions as deal with them as if they are constants in our code, which is nice.

There is a nice video that I recommend watching which is about functional programming, [check it here](https://youtu.be/e-5obm1G_FY).

------------------------------

## Modules and require()

1. Again, before taling about modules as a mere concept, I would like to simply explain the reason we need modules in the first place. Well, as programs grow and become more and more complex, especially when they depend on a huge number of other pieces of code (dependencies), it becomes harder and harder to test, debug or even add new functionality to those programs, so the concept of a module was introduced, in order to allow us to organise the pieces of code, which provide a well defined functionality to other code, we become able to reuse those modules as much as we like and independently of the program they are used in. Modules are just normal js files, talking about js specifically, they specify the programs or the other modules that depend on it, as it also exposes and interface for making use of its functionality.

2. require() is function that is  used by so many packages on NPM, it allows us to load modules and make sure that their interface is returned. Modules also preserve thier own scope, meaning that we usually do not face conflicts or anything similar to that with our own code. Using require(), modules put thier interface in an object bound to **exports**.

To simply load a module, we do the following:
```
const package = require('module-name');
```

To export a function for example, we can do it this way:
```
exports.myfunc = (itm) => itm.doSomething(); // in a file called myModule
```

Now, to use that function from that module:
```
const myModule = require('myModule');
myModule.myfunc('test'); // this will execute myfunc as if it is defined inside the code I am working with
```
We can do a lot more, like exporting one value or functionality at a time.

3. We can bring another module into the file the we are working in by eiher using `exports.value = myvalue` in case we want to load the entire interface and export a values or functions separately, or using `module.exports = value` to use a single value by overwriting module.exports. Then, we can do as follows to bring a module into out file: `const myModule = require('myModule');` or `someModule.reqFunc('test')` in case the whole interface is loaded and we used exports.value.

4. To make a module available we will have to write it into the exports object before actually using it in another file.