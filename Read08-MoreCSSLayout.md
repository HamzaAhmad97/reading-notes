# CSS LAYOUTS

## Block-Level Elements & Inline Elements

In HTML, every element is surrounded or actually rendered as a box, this box surrounds the element, its content, padding and margin and any other added borders. Elements behave differently though, **block** elements always start on a new line even if the content is just a dot, while **inline** elements flow between surrounding text, or in other words, everything that flows like a text will surround that element.

![block inline](https://res.cloudinary.com/practicaldev/image/fetch/s--1AHNQEX1--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/cvmm4upglik4tgf4azse.png)

In addition to these elements that only represent one kind of content, there are other types of elements that are known as **container** elements which are used to contain a number of regular elements. These containers can themselves be of block or inline display as well.

## Positioning

Elements if they do not get positioned using CSS they will flow normally in the same order they were marked up, however you can always alter that. There are other two known ways or modes of positioning which are relative and absolute positioning. Absolutely positioned elements get removed from the normal flow entirely, and get positioned relative to the relatively positioned parent, on the other hand, relatively positioned elements get positioned relative to their original position in the normal flow and other elements stay in their places. For the absolutely positioned elements, there is a property called the **z-index** and it is used to alter the stacking of elements when they overlap.

You can also make the element fixed, so even if you scroll, the element will stay in its place, another one is the sticky position, which is somehow similar to fixed positioning, but the difference is that the element moves or scrolls relative to its container.

You can also position elements by making them float, either to the right or the left, and once you float an elements, text will wrap around it just like water, but be careful,  since if you float all child elements in a container, the container will close up to height zero and will cause the elements to overflow or hang in there in the middle of nowhere.

All of these methods for positioning allow you to create layouts of various types and shapes, and among the most popular ones are fixed width layouts, liquid layouts and layouts that are based on grids.

![positioning](https://cdn.educba.com/academy/wp-content/uploads/2019/12/CSS-Position.jpg)
