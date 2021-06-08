## Linking in HTML

Well, the first letter of the word, or combination of words, is H which stands for hyperlinks, which as we know refers to connections or links between two sections,  elements or pages.

In HTML, you basically use the anchor tag **a** to connect to other parts on the same page, other pages, or resources you might need in your project. Basically, to use the anchor tag correctly, you will have to provide the url or the **path** for the thing you aim to reach as a value for the **href** attribute, regardless if it is some image, section in your own web page, or an external web page. Between the closing and opening tags of the anchor tag lies the content that will actually appear to the user, and most of the time it will be in blue, and underlined, but you can alter this using style sheets.

This is the basic structure of the anchor tag:

`<a href="path">Content</a>`

Speaking of the path, you have to take into consideration the location of the thing you want to connect to, for example, if it was an external website, all you need is to copy and paste the whole url of that website and put it there, however, when we talk about files and pages withing a certain directory that holds all of your project's files, then you should consider the **relative** path. The following code snippets explain this more clearly:

* Suppose that we are now in a file that is located inside a directory names main, and the file we want to reach is located in another directory directly inside our parent directory, then to reach that file, we do as follow:

`main/childDir/ourFile.sth`

* However, if the file we are looking for is located inside a directory that is on a higher level, say directly above, then we might reach it this way:

`../ourFile.sth`

Uses of the anchor element do not stop here, you can also link to a specific part of your current page by including a **#** followed by the **id** value of that element like this:

`... href="#main" ...`

You can also use differnt versions or do some additions to the href attribute to allow more accessibility. As an example, you can use **mailto** followed by an email to allow your os to open the suitable app to send an email, the same applies to phone numbers.

Other, less specific things are related to how you choose the new page that you have linked to, by modifying the **target** attribute, so for example, if you choose **_blank** when you click on the link, it will open a new tap in your browser for that page.

## Positioning and layout

HTML pages are just a combination of elements that hold content, and they usually appear in the same order they were entered in the markup, however, this is usually dull and ugly, and sometimes not practical since it might lead your content not to be easily readable or visible.

In HTML we just markup the elements that we want to show on screen, then comes CSS, CSS allows us to resize elements and position them as we see fit. But before, we have to consider the three main positioning schemes. The first is the normal one, which is basically the one we talked about in the paragraph above, the second one is relative positioning, which allows you to position an element relative to its normal position in the normal flow, but bear in mind that when the element gets positioned this way the space it had before will stay as if it were not moved at all. The third way is to absolutely position, where here, the element gets positioned relative to the root element and its original space that it used to occupy before positioning will be gone. In addition to that, you will have to provide the distance from each edge, for example, I might say something like this:

`... top: 50px; left:50px; ...`

The other way that you can position elements with is by letting them float. By letting an element float we mean that it will get surrounded by the inline and block elements like text as if the element is submerged in water on the surface.

## Functions and scopes

In general, defining a function the same way explained above will make the function available to the whole code, meaning that it can get called from anywhere inside your code, however, if you use the other ways to define functions and assign then to variables, you will have to define or declare that function above any line of code that might need to call this function or you might get an error.

`let myFunc = function func(x,y) {`

  `return x + y`

`}`

### The stack

In simple terms, the stack acts like a virtual table that holds the order all functions in your code are being executed.  

### Recursion  

Recursion stands for the action of a function calling itself, and usually this behaviour is defined inside the body of the function. Care need to be taken though, since misusing recursion may overflow the stack and make your machine run out of memory.

### Closure

Closure means that nested functions, or functions that are defined inside other functions will have full access to the variables defined inside the outer function, however, the outer function does not have the same functionality.

## Pair programming

Pair programming refers to the act of collaboration between fellow programmers on order to solve an issue or build a project. In simple terms, it is like the driver and the navigator as **Code Fellows** state it, where one of the two handles the coding stuff and the second one handles the logistics, searching, and documentation. This has proven to be much efficient since each one in a pair gets to focus more on the part he or she is handling resulting with better results and saving time.
