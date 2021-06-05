Read: 01 - Introductory HTML and JavaScript

# Introductory HTML and JavaScript

![js and html](https://ddatlearntocode.netlify.app/static/4.1-website-layers-87f0997df72de6c9754942f70f5cccef-6f0d8.png)

## HOW THE WEB WORKS?
You first type the domain name or the website you want to access, then a DNS server or a domain name server provides your machine with necessary information to access this website, then your machine sends the request to the server hosting the files for the website you mean to access, the hosting server then responds and sends back the website's documents, once your machine receives these files, the browser you used will interpret these files in order to show the website as you know it.

## STRUCTURING WEBPAGES
Web pages are built using a special language called HTML, basically, just like a newspaper, what you want to show on the screen will go inside a couple of special characters, these characters are called tags, and each element contains an opening and a closing tag, the content goes between these tags. In other words, these tags tell the browser how to display the content inside of them. Tags or elements may have attributes, which basically tells the browser more information about that element, an example of an element and an attribute are shown below.

`<img src="some url" alt="image content"/>`

Some other ways to build and moderate web pages are known as content management systems,  which are preferred by users who do not have a lot of experience in coding, these systems allow you to modify certain sections, not the whole page at once, which provides more safety at the same time, since sometimes, in coding, if you mess something up, the whole page will not show up on screen.

## OTHER HTML ELEMETS AND ATTRIBUTES

### DOCTYPE
Due to the fact that users vary when it comes to updating their browsers, but most importantly, since there was a number of HTML versions, specifying what HTML version is being used became  a necessity, thus comes the DOCTYPE element, which basically tells the browser which HTML version is being used to display the page correctly. The DOCTYPE element comes on top, before any other element, and this how it is written 

`<!DOCTYPE html>`

### COMMENTS
Some people may underestimate the power of comments, comments provide a way of telling you and the ones who are looking at your code what a certain piece of code does, and what its purpose is. Comments do not show up on the main page, they are only visible inside the source code, and they are usually written this way 

`<!-- comment goes here -->`

### Class and id attributes 
Class and id attributes are considered global attributes due to the fact that any element in the markup can include them, however, although they are used to give more uniqueness to some elements, id elements only apply on a single element, meaning that each element must only include one id attribute to preserve uniqueness, but on the other hand, the class attribute can be shared among different elements, and the purpose becomes here is to give a group of elements a unique identifier.

### Block and inline elements 
Some elements show as if they take the whole line even if they contain a single letter, these are called block elements, and some other elements do exactly the opposite, that is, they just appear as they are in the flow of the document, and only take the necessary space to fit their content.

![block and inline](https://res.cloudinary.com/practicaldev/image/fetch/s--1AHNQEX1--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/cvmm4upglik4tgf4azse.png)

### Divs and spans 
Divs and spans are general types of containers, divs are used to contain a set of block elements, while a span is used to contain a set of inline elements, so a div element will show up as a block and the span will show up as an inline element.

Iframes are used to display a webpage inside another webpage.

### The meta element  
The meta element which lives inside the head is used to show information about the page, like the author, a description,  and the type of encoding used in the webpage.

## CHARACTER ESCAPING
Since we usually use special characters to annotate text and content, we might sometimes need to actually include these characters or symbols in the actual content, so HTML provides a set of reserved keywords to show these characters in a process called escaping. It is also useful for including special characters that are not directly available on the keyboard, for example the copyright symbol which is written this way `&copy;` or `&#169;`.

## ACCESSIBILITY 
Many elements are not used to show content, but instead they are used to group elements that together give a semantic meaning, in other words, these elements help people with reader devices and search engines to look for a specific piece of content,  as a matter of fact, you can use the general containers div and span to group any set of elements, however, for accessibility purposes, it is recommended to use these elements to make your web pages more organization. Some of the example on these containers include the nav element which is used to contain navigation elements like links and buttons that play the role of directing you or the user to other pages or  specific part of the page.

## THE PROCESS OF DESIGNING A WEBPAGE
Generally speaking, it is important to put in mind that when designing a web page, you are actually designing for your audience not yourself, so you should start asking yourself questions regarding what the user is actually looking for in order to customize your webpage to provide the best experience possible.

## JAVASCRIPT AND WEB DEVELOPMENT

Javascript is programming language used to give webpages more flexibility instead of being static and dull. In general, everything in Javascript is treated as an object with a set of properties that give some object it is entity. In addition to properties, objects have something called methods, which are actually functions, but defined inside the structue of the object itself, and since methods are functons, they operate or make changes on the object like for example returning the value of a property.

Overall, Javascript is mainly used to perform these actions when it comes to web development:

* creating and interacting with objects.
* Responding to events (event handling).
* Modifying the document and its elements.

As for any other element in a HTML document, a Javascript script should be included inside the **script** element, or in an external file but in this case we will have to provide the link for that file relative to the HTML file using this script.



















