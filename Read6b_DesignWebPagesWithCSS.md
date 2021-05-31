# Styling with CSS

![CSS](https://www.freetutorialsplus.com/css-tutorial/images/css-illustration.png)

## What is CSS?

CSS stands for Cascading Style Sheets, which is a declarative syntax, not a programming language, that is used to style, position and size HTML elements, other functionalities include animation and transformation.

## Syntax

CSS style sheets usually contain a number of **rules** which themselves are broken down into **selectors** and **declarations**. The selector refers to the element that we aim to style, and there are a number of diferent types of selectors, the most simple one is the element selector, which is basically the tag name of the element. Declarations consist of **properties** and thier corresponding **values**. The image below shows the basic syntax of a CSS rule.

![rule](https://learnwebcode.com/wp-content/uploads/2010/02/anatomy-of-a-css-rule.gif)

## CSS and HTML

There are a number of ways that you can implement a set of style rules, they are almost the same since we use the `<style>` element to say that we are using a style sheet:

1. **Inline CSS**: is the most specific type of styles since it has the highest proiorities. You just use **script** as an attribute inside the openning tag of an element. 

`<p style="color: red;">...</p>`

2. **Internal CSS**: you include the style rules also in the style element but the difference here is that it must be included in the `<head>` element.

`<head>`

`<style> p {color: red;} </style>` 

`</head>`

3. **External CSS**: also included in the `<head>` element but here we do not actually add the rules between the tags of the style element, but instead we add the href attribute in the tag of the link element and provide the url for the style sheet.

`<link rel="stylesheet" href="mystyle.css">`

> Edited by Hamza Ahmad on the 31st of May.