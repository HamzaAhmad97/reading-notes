## CREATING STUNNING ANIMATED CHARTS WITH CHART.JS

charts are better than tables
chart.js relies on HTML's canvas 
bar charts, line charts, pie charts and more

drawing a line chart
1. create a canvas element in html
`<canvas id="buyers" width="600" height="400"></canvas>`

2. retreive the context of the canvas in js
  var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
3. inside the script define an object that holds the data like the labels for the x-axis and some properties

Charts sometimes carry more information than text or tables, and HTML, CSS and Javascipt combined allow us to create elegent charts like bar charts, line charts, pie charts and more, and this is using **Chart.js**. This is done using the **canvas** element in HTML, which allows you not to just draw charts, but almost anything else you want.

As a simple example, consider drawing a line chart, we will generally follow these steps:

1. Create the canvas element in the HTML file.

`<canvas id="buyers" width="600" height="400"></canvas>`

2. Retrieve the context of the canvas in the corresponding JavaScript file.

`var buyers = document.getElementById('buyers').getContext('2d');`

`new Chart(buyers).Line(buyerData);`

Where in the first line you just reference the canvas and define or set the context, where here it is 2D since we are creating a 2D plot or graph. In the second line, we create a new chart and specify the type of the chart, here it is a line chart just as we want, in addition to this, we pass the object holding the data for us to the line method.

3. Now we define the object holding the data that was passed as an argument in the previous line.

` var buyerData = { `

`   labels : ["January","February","March","April","May","June"], `

`   datasets : [ `

`     { `

`       fillColor : "rgba(172,194,132,0.4)", `

`       strokeColor : "#ACC26D", `

`       pointColor : "#fff", `

`       pointStrokeColor : "#9DB86D",`

`       data : [203,156,99,251,305,247] `

`     }]} `

As you can see, in the first key-value pair we define the labels for the horizontal axis, while in the second pair, we define other properties for the line including its color, in addtion to the data that will be used to sefine the height for each corresponding point on the axis.

Basically, the rest of the charts can be drawn the same way, but the differences include the way the data and properties are defined in addition to specifying the type of the chart. A chart drawn this way can look similar to this:

![chart](https://miro.medium.com/max/1366/1*7YTYwXJjAJ86gcNUIpvB-g.png)

You can install Chart.js using npm Node Package Manager, and [this](https://www.chartjs.org/docs/latest/) website can help you follow along with the instructions.

## THE CANVAS ELEMENT

like img but no src or alt
has only two attributes, width and height (300 by 150) by default
can be styled like any other image, including margin border and so on
always provide a fallback since not always supported by older browsers the fallback is inserted inside the canvas element itself

#### The Rendering Context 


The canvas element is similar to an image element in a way but it does not have a src nor an alt attribute, it only has two optional properties which are only the width and height of the canvas element, and by default they are 300px and 150px. The canvas element can also be styled like any other image element including its margin, padding and so on. Another thing to take into consideration is that the canvas element can be sometimes not supported by older browsers, so it is recommended to provide some fallbacks like images or text between the opening and closing tags of the canvas element.

To start drawing, in addition to referencing the canvas node just like any other element, you will have to access the **rendering context** to draw on it. You can access the rendering context of a canvas by using the `getContext()` method, and you will only have to pass one argument to this method, which is the type of the context, for example, for 2D drawings, you will have to pass "2d"

`ctx.fillStyle = 'rgb(200, 0, 0)';`

`ctx.fillRect(10, 10, 50, 50);`

As you can see from the two lines above, which allow us to draw a rectangle, you specify the way you want to color the thing you want to draw in the first line, here it is using RGB, and in the second line, we use the context to draw a rectangle using the **fillRect()** method specifying the coordinates of the four corner points. A typical result might look something like this:

![rect](https://lh3.googleusercontent.com/proxy/Z9cDJa-zJKy2YOKFHMB984jgBFGg989IzQC1WCvCb-aUrnoe96-ZFgXn5B9j4e0qDizRwWtg9n40qlvdKfcyV9C6TcykMpZDH_w4ZIUbtv-6xPoNHk2SIauB)

You can check [this short tutorial](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage) to start playing with the canvas element.

#### Drawing Shapes With Canvas

working with paths, 

###### The grid

Since canvas relies on paths for drawing shapes, we have to give extra attention to the grid, which simply can be explained as follows:

We first define the width and height of the canvas in pixels, you can think of all the pixels as being very small squares. Starting from the top left corner, each time we move either left or right we add one depending on the number of squares we cross, so for example, if we move to the right 5 squares and to the bottom 5 squares, our coordinates will be (5,5), the x-axis is directly related to the horizontal direction, while the y-axis is related to the vertical motion. A grid might look something like this:

![grid](https://forum.bpmn.io/uploads/default/original/1X/5e3ed8d11a1f6bdccc2fc4e10af170fc8831accb.PNG)

###### Drawing rectangles

Since canvas only supports drawing rectangles and paths by default, it is useful to introduce some of the methods used to draw or clear rectangles. Note that all the positons or coordinates specified are relative to the top left corner.

* `fillRect(x, y, width, height)`: draws a filled rectangle.
* `strokeRect(x, y, width, height)`: draws a rectangle outline.
* `clearRect(x, y, width, height)`: clears the specified rectangle area.


###### Drawing paths

Using paths, you can break the barier and start drawing more complex shapes than rectangles. A path is simply a path or a line connecting multiple points. To make shapes using paths, you will have to first create the path itself, then use some of the drawing commands to draw into the path, and lastly, you can stroke the path or simply fill it to render it. Some of the functions used to do these steps are:

`beginPath()`

`Path methods`

` closePath()`

This also allows you to draw arcs, Bezier and quadratic curves and any other combination from them.


#### Applying Styles and Colors

You can use color with canvas using properties like `fillStyle = color` which sets the style used when filling the shapes, and `strokeStyle = color` which sets the style of shapes' outlines. You can use the same values used in CSS documents to set colors. You can also change or modify the transparency and line widths and so on.

Check [this website](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors) for more information and examples.

#### Drawing Text

To draw text, you can use the `fillText(text, x, y [, maxWidth])` method which allows you to fill the given text at the given (x,y) position, and the `strokeText(text, x, y [, maxWidth])` method which allows you to stroke the given text at the given (x,y) position. There are other properties that allow you to change the style, alignment, line height and the direction of the text.







