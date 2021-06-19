## Images

As for any other element in the HTML document, images also can have lots of preperties that can be changed like size and position.

### Modifying size
To modify the size of an image, you can set the width and height attributes in the image tag, and this gives you some fast way to change the size of an image, however, this is not the optimal way, since you might run into trouble especially if you want the image to resize and adapt to the size of the container. The other similar way includes using also the width and height properties in the CSS document.

### Aligning and positioning images

You can simply let images float, to the right or to the left, and let text wrap around the image, as you also can center an image using a couple of methods, the first one includes giving the image a block display property, and giving it an auto margin in the direction where you want to center it, however, we learned even better ways, and one of them included using the flex display property and using the align-items or justify-content to center the image.

### Images as backgrounds

Images can also be used for decoration purposes, like being used as a background for some other element, using the background-image or simply the shorthand background property allows you to do that, you can also control the behaviour of the background, like if you want it to repeat if it does not fit the container using the background-repeat property, you have the choice of specfying the direction of repetition. You also have the choice of letting the background stay stationary and scroll with the element or just stay stationary using the background-attachment property. The background-positon property allows you to specify the location where the backgound image will appear, this effect will be most visible when the background image is narrower than the container.

You can also let the color or the background of an element to be a gradient, a linear one or a radial one using the linear-gradient or radial-gradient values.

A lot more than this can be done with images, however, the one should take into consideration other properties inherit in the image itself, like the colors it contains, contrast, brightness, and many more.

## Search engine optimization

Search engine optimization or simply SEO is a topic concerned with making your website as much accessible as possible by using a couple of tecniques which can be sorted into two main categories, the first one is on-page techniques which includes takeing care of what is being written in text like keywords and so on by trying to think about what terms people will use when searching for a webpage that matches thier needs. The other method which is called the off-page techniques, which includes the other wabpages linking to your webpage, and all of these play a major role in making your webpage more visible by search engines.

To apply this on your website, you will have to consider many things related to the strcture of your webpage, and that's why it is recommended to use tags that carry a semantic meaning when structuring your page. In addition to this, you should start asking yourself questions related to the nature of the visitors or potintial ones, like language, and if they are going to be frequent visitors or just unique ones and so on.

## Video and Audio APIs

HTML allows you not oonly to include images and texts, but also, you can add videos and sounds to your website. To add a video for example you will have to use the **video** tag which works as a container for a set of videos in case a browser does not support one the formats. To add a video, you may add something like this:

`<video controls> <source src="myVideo.mp4"></video>`

The controls attribute allows you to show the controls bar in the bottom section of the video, but usually they are based on the browser, and might not be that functional, so as recommended, it is better to use or build your own controls, or use the HTMLMediaElement API that allows you to control video and audio programmatically, for more info, you can check [this MDN article](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs).


This API implements fairly simple HTML, CSS and Javascript codes that allow you to modify the style of the controls, seek forwards and backwards and so on.

![](https://cdn-media-1.freecodecamp.org/images/1*FKJojPyvDky1kM3gK5Z7KA.png)