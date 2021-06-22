# TRANSFORMS, TRANSITIONS AND ANIMATIONS

## Transforms

In a sense, the transformations in CSS is somehow related to linear transformation from linear algebra operating on a vector in a vector space and transforms it based on the nature of the linear transformation itself. Transformations allow us to stretch elements, scale them and rotate them. In CSS, all of this is done using the **transform** property which accepts a number of transformation functions that do something special to an element. In addition, these transformations can be done in 2D or 3D spaces.

### 2D transformations  

* Rotation

To rotate an element, you will have to use the **rotate()** value, which accepts one argument which is the angle of rotation, the angle can be positive, indicating counter clockwise, or negative, indicating, clockwise. The center of rotation is the center of the element by default however, you can always change the center or origin or rotation, example: `transform: rotate(20deg);`.

* Scaling

You can also scale, or change the "apparent" size of an element using the value **scale()**, which also accepts one argument which represents the amount of scaling, so for example if you supply the value 0.5, the element will show up shrunk by half, knowing that this value ranges between 0.1 and 1. Notice that this scaling does not actually change the actual width and height of the element in the flow, but instead, it only changes the way the element gets rendered. You can also scale an element in one direction, either in the x or the y direction, making the element appear to be stretched or squished, example: `transform: scale(.75);`.

* Translation

Translation in CSS works pretty much the same way as relative positioning, the space the element occupies in the normal flow is preserved, but the element is free to get positioned without changing the organization of the document. Using the **translate()** value, you will be able to position an element reltive to its original position, you can also translate in a specific direction, the x axis or the y axis, example: `transform: translate(-10px, 25%);`.

* Skewing

Skewing is like applying a shear force on the edge of an element, it is like when you gently push the surface of a jelly cube and watching its shape getting distorted, in CSS you can do this in one direction or in both using the **skew()** property, example: `transform: skew(5deg, -20deg);`.

An element can accept more than one transforming value, it can be translated and rotated at the same time and so on. You can see below an image showing some samples about transformations in CSS.

![2D transforms](https://html-css-js.com/images/tiles/css-transform.jpg)

### 3D transformations  

As per the [MDN website](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/perspective()), The **perspective()** CSS function defines a transformation that sets the distance between the user and the z=0 plane, the perspective from which the viewer would be if the 2-dimensional interface were 3-dimensional. This property can be applied on the element itself or on the parent which is useful if you aim to apply the transformation on a group of elements, and once you supply the perspective property, you can use the other transformation properties discussed before like rotation.

Since the perspective property accepts none or a measurement value like **px**, we can talk about the depth of the perspective. It kind of changes how far or close the horizon or the the distance the element is away from us, example: `transform: perspective(1000px) rotateX(45deg);`. the origin of a perspective identifies the coordinates of the vanishing point of a transform, example: `perspective-origin: 75% 75%;`.

Basically, for 3D transforms, you can do almost the same as with 2D transforms, the only difference is that here we are taking the z direction into consideration. Below you can see a sample of some of the 3D transformations.

![3D](https://tipsmake.com/data/images/3d-transform-in-css-picture-1-jtznOkrOW.jpg)

## Transitions & Animations

We can think of transforms as happening in only one frame or at only one point in time, where the element stays stationary when its appearance is changed. Transitions and animations allow us to make elements change shape and appearance continually and or when they get hovered over or clicked and so on.

### Transitions

For transitions to work the element has to undergo a change in state, like being clicked for example, and this can be done using pseudo classes, which can be thought of as if the element at some stage or status it then belongs to a special class, some of the most known pseudo classes are **hover**, **focus** and **active**.

Transition properties are:


* transition-property.

* transition-duration.

* transition-timing-function.

* transition-delay.

The first properrty selects the property that we are going to do the animation with, or in other words, the property that will undergo an animation or a change in value over a specified period of time. The second property defines or determines the duration the transition is going to take, the third property defines a function that will govern the way the transition progresses over time, so if you remember the linear function, which shows a 1:1 relation between the x and y axis, the animation will progress smoothly and with the same pace from the beginning till the end. The last property is the transition delay which simply makes postpones the animation for a specified period of time. It is worth noting that not all properties are supported by transitions, so you might need to look that over.

### Animations  

When heavy duty or top-tier animations are needed.

#### Keyframes animations  

To start, we use the **keyframes** rule to build or define animations, simply, to define an animation using keyframes, we add the keyframes rule, the animation name, and then any break points needed along with the properties to be changed in each one, a typical simple example of keyframes animations might look like this:

![KF](https://www.imore.com/sites/imore.com/files/styles/xlarge/public/field/image/2014/11/understanding_css_animations_03.jpeg?itok=Qdn5mQQc)

For keyframes animations, you almost have the same properties used for transitions, you can specify the duration of the animation, he timing function and the delay. In addition to all of these, you can also specify other properties, like the animation fill mode, which simply lets you decide if you want the element undergoing the animation to stay at the last state it reached.
