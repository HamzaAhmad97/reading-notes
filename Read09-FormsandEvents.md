## Forms 

You almost never go across a website and do not encounter a form or at least a form element, every button, text field or a drop down menu, all of these are part of forms. Basically, forms allow you, the host, to collect information about the user interacting with your website, in addition to this, they also provide a way for the user to gain more optimized features or an environment that is more aligned with his or her preferences, they are also used to track changes and store them in a server to avoid losing data. There are a number of ways that you ususally interact with forms, you can select one or many choices or options from a list or a drop down menu, you can enter text as you also can click buttons, a typical example might look like this:

![simple form](https://www.w3.org/TR/html401/images/form_exmpl.gif)


Basically, when a form is submitted, the name and the corresponding value of the element that was filled or chosen gets sent to the server, the server process the data and responds accordingly.

The basic structure of form will mostly include the form element, which acts like the container for the other form elements or controls, in additon to this, the form element has two important attributes, namely, the **method** and the **action** attributes. The action attribute holds the URL for a specific page in the server, while the method attribute holds one of two distinct values, **GET** and **POST**, where if the GET mode is chosen, then the content or the values of the controls will be appended to the URL specified in the action attribute, while on the other hand, if it is set to POST, the data will be sent privatly.

![getpost](https://img-cdn.majarah.com/post/3510199940050963_26971843608098_7512635124163186_9817879398918998_Majarah_tech_.png)

There are a variety of controls or form elements, but they all share the same behaviour regardless of the nature of their input, since all that matters is to send the name of the input along with its value. All of these elements have special attributes that allow you to customize them like setting the maximum allowble number of characters to be typed inside a text field and so on. The list below shows a number of form controls or elements:

* `<input type='text'>`: used for text input, and can be adjusted to accept specific types of entries like a password or an email.
* `<textarea>`: also for text but usually for entries that might span more than one line.
* `<input type="radio">`: radio button, where you can only select one.
* `<input type="checkbox">`: checkboxes, where you can choose more than one.
* `<select><option>... </option></select>`: a dropdown menu with options.


As you also have much more than those, like for uploading a file, buttons and so on. There is the **label** element which used to give labels for form controls, and its role is purely aimed to be for accessibility purposes.

## Styling Lists, Tables & Forms

As for any element in a HTML document, lists, forms and tables can be styled and modified in a number of ways, lists for example can have thier bullet points or numbers modified to be in different shapes, as they also can be images. Forms can have the color of the cursor in an input field changed, and tables can have alternating colors for rows. I will list all of the properties that can be changed for each one of these elements, but I will only list 3 for each one, and you can always check the book or the W3school website for a reference on these properties.

1. Lists
* list-style-type: change the shape of the bullet points.
* list-style-image: change the bullet points to be an image.
* list-style-position: adjust the positon of the bullets, like either hanging or inside.

2. Tables

Tables can be considered like any other block element, they can have thier width, height and thier background color changed, and the same applies to the row elements and cell elements, td and th.

3. Forms

Almost what applies to tables applies to forms in additon to the ability to modify the shape and color of the cursor.

## Events

Events are basically tied to the action of doing something, and we say that an event has occured, but in a more technical terminology, we say that an event has fired or raised just like we do with errors. Usually, we wait for events in order to do something related, so for example, we might want to have the page show something when the user clicks (event of clicking) something.

Types of events:

* Form elements.
* Focus events.
* Mutation events (related to modifications to the DOM).
* UI events.
* Keyboard events.
* Mouse events.

In order to make use of an event listener, you select an element node, you indicate which event will triger the response and then you construct the code that will run when the event occurs.


To get an element to trigger some piece of code when an event occurs, you can set one of the traditional DOM event handlers, which can be included in the opening tag of an element like this way `...onClick="someFunction()"...` as you can also do the same in the JavaScript document. The other more effecient way is to assign an event listener in addition to the callback function all in one line of code using the **addEventListener()** method. which accepts the type of the event, a callback function, and another optional argument for controlling the flow or the propagation of the event.

`element.addEventListener('mousedown', someFunction);`

There is also a propert unique to events and event listeners, and that is that thry propagate and bubble to other containing parent elements, but that can be useful for so many reasons as it is also can be adjusted or even prevented.
