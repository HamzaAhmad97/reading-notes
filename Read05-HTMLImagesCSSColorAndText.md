## HTML Images 

Images in HTML can be used to add important or vital information when it comes to websites, mainly, there are two main uses for images, they can be merely decoratvie, and they can be used to give extra emphasis to some a particular suject.

To add images to your page, you can use the **img** tag, you will usually have to add the **src** attribute and add the path or the url of the image you want to include, they can be part of your project or they can be linked by getting thier address online. For accessibility purposes, it is recommended that you add an alternative describtion to the images you add to your page using the **alt** attribute such that if something goes wrong, or if the browser fails to retrieve the imge and nothing shows up this alternative describiton will be there telling that an image was supposed to be there.

You can also specify the width and height of any image you add using the width and height attributes, but it is recommended to do that using CSS. Many factors should be considered when choosing images for websites, among them is the content of the image itself, in addition to the size, resolution, and the way the image should be cropped based on the media quiries you implement, and all of that plays a major role in adding a sense of responsiveness to your website.

This is the tag for adding images:

`<img src="path" alt="alternative describtion">`

## Colors

Colors is a vast area to be fully covered, but in short, colors are usually concerned with the front and background color of some element, it is also related to topics like opacity. There are a number of ways to add colors to an element, and they are listed below:

* Named Colors

* RGB

* RGBA

* HSL

* HSLA

The first method requires you to only name the color you want to use as a value for the color or the background-color properties, you can think of them as if they are a predefined set of colors and they are ready to be used at anytime. The RGB system uses a combination of red, green and blue to produce a color, you can use **rgb()** to add the 8 bit color value (255) to specify the amount of each color or the hex notation like **#FFFFFF** for example. The HSL is a bit different, but not that much, but mainly, it deals with hue, saturation and luminusity or lightness, but here you will have to take a look at the circle of color to enter the "radial" coordinates of the color you want in terms of hue, saturation and luminusity.

The 'a' at the end of HSLA and RGBA refers to the opacity or the transparency of the color.

## Text

When it comes to text, we can mostly talk about how we can alter the presenttion of text, and here is a list of properties and thier uses in CSS:

* font-size: used to change the size of the font.

* font-family: used to select a set of fonts to change the overall shape of text.

* font-decoration: used to add some decoration to text, like underlining.

* text-align: used to change how the text spreads out.

* letter and word spacing: used to change the amount of space between letters and words.

* text-indent: to change the amount of space before the first line of text.

There are much more than those properties, but you can look them up online whenever you need.

## Image Formats

1. **JPEG (.jpg, .jpeg)**

JPEG, which stands for Joint Photographic Experts Groups is a “lossy” format meaning that the image is compressed to make a smaller file. The compression does create a loss in quality but this loss is generally not noticeable. JPEG files are very common on the Internet and JPEG is a popular format for digital cameras - making it ideal for web use and non-professional prints.

2. **GIF (.gif)**

GIF or Graphics Interchange Format files are widely used for web graphics, because they are limited to only 256 colors, can allow for transparency, and can be animated. GIF files are typically small is size and are very portable. 

3. **PNG (.png)**

PNG or Portable Network Graphics files are a lossless image format originally designed to improve upon and replace the gif format. PNG files are able to handle up to 16 million colors, unlike the 256 colors supported by GIF.
