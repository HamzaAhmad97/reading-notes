## The problem domain

In simple terms, understansding the problem domain is all about understanding the problem itself. Starting with the solution for a problem without clearly understanding the problem domain is like driving a car not knowing the destination. The problem domain limits the amount or number of things you will have to consider when working on a solution, for example, sometimes when coding, if the problem you are working on is purely algorethmic then you might not need to use any library, however, if you did not understad the problem clearly, then you might need to use a number of libraries and thus wasting time for no good use. So, understanding the problem domain should be the first step when working on any problem since it allows you to focus all of your efforts and resources on the problem and save you time and resources.

## Objects and the literal notation for creating them

You can think of anything as an object, since everything has properties like for example if it is a living thing or not, in addition to methods that define the behaviour, for example, cats "meow" and so on, in fact that's almost all you need to know about objects.

In order to define an object, you can use the literal notation or the constructor which will br descussed in other readings. To define an object you use a couple of curly braces and between them, you define the properties and the methods you want to include for the object, note that properties are basically some of the variables we used before to store values, and methods are also just functions that allow us to interact with the object or to make the object itself interactive.

1. ` let cat = {`
2. `    age: 1,`
3. `    meow: function() {`
`    console.log('meow');`
`      }`

4. `}`

In line 1 we define a variable to hold a reference to our object and we named it cat, and in the second line we defined a property named age which only saves the age of the cat as a number, and lastly, we defined a variable named meow to hold a reference to a function that does something, thus a method, then we close the curly braces.

## The document object model 

The document object model or just the DOM is basically a model that has tree-like structure, and the leafs are called nodes, this model basically allows us to modify our page and its elements and alter its behaviour as we like, the image below shows an example of this model:


![DOM](https://i.morioh.com/200725/6b050937.webp)

There are four main types of nodes in the document object model, and the are listed below:

* Root (document) node: which simply represents the whole page or the HTML element.
* Element nodes: which basically defines the structure of the HTML page like the paragraph element for example.
* Attribute nodes: which refer to or represent the attributes of an element which can be found in the opening tag of an element.
* Text nodes: carries the text inside of an element node.

## Working with the DOM

Mainly, you will have to access an element or an array or a list of nodes, and once you locate them, you might be thinking about modifying thier attributes or content or even styles. Accessing nodes is itself concerned with either accessing a single element, a nodelist or moving though elements or nodes, and these three actions can be done using methods and properties like theses:

- getElementById(id): to access a node by its id value.
- querySelectorAll(context): basically takes a selector to access an element or a set of elements that match that selector.
- parentNode: to access the parent node of some node.

The other part of the story is concerned with dealing with the those nodes or elements once we locate them, and that includes either getting or updating theier content or attributes, working with HTML content or thier children, or accessing and updating attributes values, and the following methods and properties allow us to do such actions:

- nodeValue: access or update the content inside any child element.
- createElement(): allows you to create empty elements by providing their type.
- getAttribute(): get a specific attribute of an element.

Usually, it is recommended that you store the location or the reference to the elements you locate inside variables in order to reduce the amount of code and not to waste time in a process called cashing, which also affects the performance of your website.

These methods and attributes allow you to do almost whatever you want with your page, starting from selecting elements based on the value of thier attributes like their class or id, or based on their location in the DOM which is done using query selectors, as you also have the ability to select a number of elements in a nodeList.

