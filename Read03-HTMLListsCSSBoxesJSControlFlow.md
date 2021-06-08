## Lists in HTML

In HTML there are a number of different types of lists, you can use any of them, however, it is recommended that you use the one that mostly agrees with the nature of information you aim to present.

* Ordered lists

Which shows numbers indicating order for every list item, for example, it is best suited for steps.

`<ol>`

`<li>Hit</li>`

`<li>Run</li>`

`</ol>`

The list will show up like this:

1.Hit

2.Run

---
* Unordered lists

Can be used almost for any type or shape of information that needs to be listed since the list items will not be numbered or indexed.

`<ul>`

`<li>Hit</li>`

`<li>Run</li>`

`</ul>`

The list will show up like this:

* Hit

* Run

---
* Definition list

Used to represent a list of terms and thier definitions, or for list items that may need to be explaind further.

`<dl>`

`<dt>Term</dt>`

`<dd>Definition</dd>`

`</dl>`

The content within the **dt** element is the term, while the content within the **dd** element is the definition of the term.

Lists of all shapes and types can be nested within each other to form what is known as nested lists, and they can be of multiple levels.

## Thinking inside the box

There is something called the box model, it is basically the real space that each element takes when we reveil its margin and padding. As you can see in the image below, this box model consists of three main regions; the actual content lives inside the content box and never exceeds it, the next box surrounding the content box is the paddind box or padding area, and together, they are surrounded by a border. The most outer area is the margin area, and although we add margin to elements but actually it can be thought of as the pushing area around the element, where no other element should pass or touch aside from the outer edge. You can modify and adjust a lot of the properties for these areas like the padding, the border width, the amount of margin and so on, as you can specify which area to size using the box sizing style property.

![Box model](https://codinglead.github.io/images/box-model.png)

## JavaScript Arrays

Arrays are a very popular data structure that is used to hold or contain a number of other more basic data types and even other data structures, the syntax to define an array is as follows:

`let myArr = [1,2,3,4,[5,6,7]];`

Basically, and array is a pair of square brackets, and between them are the values we want to contain separated by commas.

## If else statements

If else statements are control flow statements, basically, you include a conditon bewteen the parantheses after the if keyword, and if the result of that condition is true, the block of code following will get executed, otherwise, if the else block will get executed.

## Switch statement

The switch statement is used when we have some expression, and based on the value of that expression we might need to do something specific to that particular value, you may feel tempted to say that we can use the if else statement, and you are correct, however, things cam get dirty so fast, and your code can get bulky and ugly and hard to read, so a switch statement helps in reducing the pain and time of doing the same thing with if else statements.

![switch](https://www.tutorialspoint.com/javascript/images/switch_case.jpg)

## Truthy and falsy values

We all are familiar with the Boolean values true, and false, but what happens when you compare **null** to 3 for example, does javascript break? In fact it never complains, since there are values that are dealt with as if they are false, and others like the number 1 are condidered true.

## Short-circuiting

In short, short circuiting refers to the act of ignoring the other value on the other side once we make sure that the first value is falsy when we are talking about **and**, or when the first value is truthy when we talk about **or**. Basically, if we had and, and the first value is evaluates to false, then JS will skip the other value and ignore it, while if we had or, and the first value is truthy, then JS will skip and ignore the second value, provided that it does not result with a syntax error.


## Loops

Most of the time, you will need a peice of code to execute for a number of times, sometimes you find it easy to type the commandsor linesof code by hand manually when the number of loops or iterations is fairly small, however, things can get so tiring so quickly once the number of iterations increase, so you start to feel the urge to automate such tasks, and thus comesthe term of looping.

As in any other programming language, Javascript offers a number of ways that allow you to loop or iterate in order to execute a peice of code. The list below shows the most common loops in Javascript:

* for statement
* do...while statement
* while statement

As an example, the following code snippit, shows the general syntax for a for loop:

`for ([initialExpression]; [conditionExpression];[incrementExpression]){`

  `statement`

`}`

Edited on June 8th