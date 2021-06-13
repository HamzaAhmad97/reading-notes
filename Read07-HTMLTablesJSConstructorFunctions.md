## Domain Modeling

Domain model is a structured visual representation of interconnected concepts or real world objects that incorporates vocabulary, key concepts, behavior, and relationships of all of its entities, and it mainly focuses on the visual aspect since our brains are better at memorizing and learning things using imaginetive constructs.

In coding, it is more like thinking of what you build from functions to objects as if they are things that exist in real life, and you start to better connect them and understand how they unteract with each other.

## HTML Tables 

Tables allow us to present information in a meaningful way by organizing them through rows and columns, and each of these rows and columns intersect at a singel cell. Usually in tables, rows and columns are labelled to reflect or make it easier to work and understand data.

To mark up a table in HTML, you will start with the **table** element which acts as a container for the **tr** element which represents a table row, which itself acts a wrapper for the **td** element or the table data element which stands for a single cell.

![table](https://www.problogdesign.com/wp-content/uploads/2009/05/descriptiontable1.gif)

The **th** element is used to add headings to columns by setting its **scope** to column, and to rows also but the scobe attribute should be changed to row. Columns can span more than one cell or column, by changing the **colspan** attribute and giving it a value you indicate that this column will span more than one cell or column, the same property is also available for rows too but the attribute itself becomes **rowspan**.

There are also a couple of elements that are mainly used for accessibility purposes for long tables and people with disabilities, which are `<thead>, <tbody>, <tfoot>` which basically act like the header, main and footer in the normal markup.

## Objecta and the constructor notation

Previously, we used the literal notation for defining objects, which after a while you will notice is impractical, especially when most of the objects share most of their properties or behavior. 

To start, you begin with the new keywork followed by the constructor function, so for example, to create an empty function, you can do the following:

`let emptObj = new Object();`

Where Object here is actually the constructor of every object there is, then after that you will be able to add properties to the object using the old dot notation or the square brackets.

The constructor looks exactly like a normal function, however, the first letter is usually capitalized. Since the constructor is actually a function, it can take a number of parameters, and these parameters are used to define the status or give the new object some behaviour once it is created, a constructor looks like this:

![costructor](https://www.codegrepper.com/codeimages/which-statement-creates-a-new-object-using-the-person-constructor-in-javascript.png)

The **this** keyword is used to refer to the object that we are working on changine its properties or making it do something, however, when it is added in the global scope it can be misused sometimes since it might be referring to the window object.

Using objects is also a great way for storing data just like we did with arrays and simple data types like numbers and strings, but objects are more functional and easier to deal with because the information or data they contain is usually labelled and you can nest other objects inside of each other.

Almost everything in Javascript is an object, even arrays and functions! Yes, functions are actually objects and they have thier own properties and methods just like any other object there is like **argument** which holds the arguments passed to a function, and the **method** that allows you to explicitly specify the "this" keyword.