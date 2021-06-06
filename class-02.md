Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions


## MARKING UP Text

### Headings 

There is a total number of 6 headings, they mainly carry a semantic meaning which is showing the main headings or titles in a HTML document. The h1 tag is used to show the main heading, while the rest, h2, h3, h4, h5 and h6 are used to show subheadings, they show up in different sizes based on the type of heading you use.

`<h1> <h2> <h3> <h4> <h5> <h6>`

### Paragraphs

The paragraph tag is used to contain regular text, and they ususally show up with the same size as for the HTML element, which is ususally 16px.

`<p>`

### Bold & Italic

Text contained in a bold tag shows up in bold, which gives a meaning of importance, while text contained in a italic tag shows up inclined, which gives the meaning that the text inside would be said in a different way from surrounding content.

`<b> <i>`

### Superscript & Subscript

Used to show characters that should be superscript or subscript, like the power in mathematical formulae, or indices when it comes to subscripts.

`<sup> <sub>`

It is a good practice to include whitespaces in order to make your code more readable, however, HTML usually ignores extra whitespaces in the same level, so we should take this into account.

### LINE BREAKS & HORIZONTAL RULES

Paragraphs show up on separate lines since they are block elements, however, using line breaks, you can add a line break inside the middle of a paragraph, and using horizontal rules, you can create a visible divider line between sections or themes.

`<br /> <hr />`

### Semantic Markup

Which basically refers to the elements that do not actually alter the structre of a document, but instead, they give extra information about the content inside them, examples are:

* `<strong>`: content inside of me has more importance.
* `<em>`: slightly more emphasis should be given to the content.
* `<blockquote>` : for long quotes.
* `<q>` : for shorter quotes.
* `<abbr>` : indicating that there is an abbriviation.
* `<cite>` : when referencing a piece of work, like an article from a book.
* `<dfn>` : explaining terminology.
* `<address>` : to contain contact info about the author.
* `<ins> <del> <s>` : indicating changes to content, like deleting content that no longer applies, showing newly added info, or indicating that a piece of content does not currently apply or it is currently irrelevant.

## Inroducing CSS

CSS stands for Cascading Style Sheets, which is a declarative syntax, not a programming language, that is used to style, position and size HTML elements, other functionalities include animation and transformation.

### Syntax

CSS style sheets usually contain a number of **rules** which themselves are broken down into **selectors** and **declarations**. The selector refers to the element that we aim to style, and there are a number of diferent types of selectors, the most simple one is the element selector, which is basically the tag name of the element. Declarations consist of **properties** and thier corresponding **values**. The image below shows the basic syntax of a CSS rule.

![rule](https://learnwebcode.com/wp-content/uploads/2010/02/anatomy-of-a-css-rule.gif)

### CSS and HTML

There are a number of ways that you can implement a set of style rules, they are almost the same since we use the `<style>` element to say that we are using a style sheet:

* **Inline CSS**: is the most specific type of styles since it has the highest proiorities. You just use **script** as an attribute inside the openning tag of an element. 

`<p style="color: red;">...</p>`

* **Internal CSS**: you include the style rules also in the style element but the difference here is that it must be included in the `<head>` element.

`<head>`

`<style> p {color: red;} </style>` 

`</head>`

* **External CSS**: also included in the `<head>` element but here we do not actually add the rules between the tags of the style element, but instead we add the href attribute in the tag of the link element and provide the url for the style sheet.

`<link rel="stylesheet" href="mystyle.css">`

## Basic JavaScript Instructions

Generaly speaking, a script is a set of instructions, more specifically, a line that is used for its side effects is usually refered to as a statement, like a print statement, on the other hand, the lines of code that are known for thier returned value are known as expressions.

### Comments

To use comments in a script, there are two main ways, the first one is for inline comments, using `//`, and the other one for multi line comments that span more than one line, and we usually use `/* */` to do that.

### Variables

Variables act like containers, some of them contain the value itself, while other hold a refernce to values not the values themselves. To declare a variable:

`let x = 5`

`const y = 3.14`

### Datatypes

There are a number of datatypes in JavaScript, like the number type which from its name is used to hold numbers, other datatypes are strings, which are used to hold any set of characters between a pair of quotation marks, also, there is the boolean datatype, which has only two valies, true and false.

### Naming Variables

There are a few set of rules regarding naming variables, among them is that a variable name must not start with a number, also, the name itself must not be a reserved word like let for example, as it also must not contain any special characters.

### Arrays

Arrays are a data structure used to contain a set of values of any type like the ones discussed before, arrays can be modified the thing that also applies the values inside of them. To define an array and access a value inside of it, you have to include a pair of square brackets after the array name.

`let myArray = [1,2,3,4]`

`let x = myArray[0] // x will be equal to 1`

### Expressions and operators

Expressions are lines of code that result with a value, usually expressions consist of a number of operators that have special functions which also operate on a number of operands to yeild the result. For example, among the logical operators is the (or) operator which operates on two boolean values and returns false if and only if both operands are false.

Types of operators:

* Assignment operators --> **Example: =**
* Comparison operators --> **Example: >**
* Arithmetic operators --> **Example: +**
* Bitwise operators --> **Example: >>>**
* Logical operators --> **Example: or**
* String operators --> **Example: +**
* Conditional (ternary) operator --> **Example:  ? :**
* Comma operator --> **Example: ,**
* Unary operators --> **Example: delete**
* Relational operators --> **Example: in**

## Decisions and Loops

Most often, we will find ourselves needing a way to alter the execution of our code, and thus comes the idea of control flow and looping.

In summary, we use a predefined set of code to do something when a condition is true and do something else when the condition is false, take for example the if else statement, which gets passed a condition, an expression that evaluates to true or false, and if the condition is ture, the block of code inside the if statement will get executed, but if the condition is false, the block of code inside the else statement will get executed.

`if (condition) {`

`	// execute this if true`

`} else {`

`	// execute this if false`

`}`

Looping simply refers to the action of executing someting a number of times, sometimes we do not the exact number so we use something called the while statement, but when we know the number of iterations, we use the for loop.

`if (counter; condition ; increment/ decrement) {`

`	// execute this many times`

`}`

