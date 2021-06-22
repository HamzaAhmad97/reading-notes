# LOCAL STORAGE

## The story

I think that at one point in your journey to become a web developer, you wanted to store the environment, which simply is the combination of states stored in variables and so on, somewhere, you are not yet profecient with server stuff, so you have no means of storing this data such that the user can access the website or the page and continue where he last left, but since we still do not know a lot about servers, you will resort to our local machines and the browser itself to store all the data we need to add some kind of continuity to the user's experience.

The most famous utility for doing this storage thing relied on something called **cookies**, but they relied on sending data over and over to the server, thus using the internet, and they also had some limitations like the limited storage capacity, and slowing down web pages and web applications.

Here is a history lesson for you about how local storage evolved over time, you can check it on [this](http://diveinto.html5doctor.com/storage.html) website.

## HTML5 Storage (Web Storage)

Rememebr objects in JavaScript? or maybe dictionaries in Python? well, the HTML5 storage is almost the same, it is a way for web pages to store named key/ value pairs in your local machine, a typical example might look like this:

` {userName: 'Albert', age: 26} `

HTML5 is accessed through the **localStorage** object on the global window object, you can check on your browser if it supports it using the **in** operator, you can use **Modernizr** for the same purpose.

### Using HTML5 storage

Just like **JSON**, the actual data is stored as a string, even if you add or supply numbers or boolean values, and to get these values as is, you might need to use some of the built-in methods to cast or convert the data to its original type. 

The syntax is similar but it is a bit different from what we are used to, however, the functionality is the same, so for example, you have setters and getters just like for objects to retrieve data or update it, and just like arrays, you can use square brackets to do the same, in addition to the ability to remove values given a named key.

` setter creator void setItem(in DOMString key, in any data); `

` var foo = localStorage["bar"]; localStorage["bar"] = foo; `

In the first line, we used setters and getters, but in the second one we used square brackets.

### Tracking changes

We have the storage event, which gets fired everytime **setItem()**, **removeItem()** or **clear()** get called and actually change something not just being called and do nothing. You can attach the event listener to the window object, and add a callback function to do something when the event is fired.