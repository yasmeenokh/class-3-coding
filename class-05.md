# **Chapter 5** 
## **Images**

**Adding images**
we use <img></img> element it has two attributes "src" tells the browser where it can find the image file, it
usually inclides a relative URL. alt is used to provide a text description of the image when the image can't be seen. 

**NOTES**
1. we use height and width to determine the image size.
2. you can place an image before a paragraph, in the middle of a paragraph, and Tin the middle of a paragraph. 
3. align attribute is used to indicate how the other parts of a page should flow around an image.
4. <figure> element is used to contain images and their caption so that the two are associated. 
5. <figcaption> element is used  to allow web page authors to add a caption to an image.

### **Rules for creating images**
* Save images in the right format.
* Save images at the right size.
* Use the correct resolution.


# **CHAPTAR 11**

## **COLOR** 
color properly allows you to specify the color of a text inside an element. 

One can choose the wanted color by three ways: 


RGB values | HEX code | color name 

-----------|----------|-----------

This express the colors in terms of how red, green, and bule are used to make it up. | These are six digit codes that represents the amount of red, green, and blue preceeded by hash. | There are 147 predifined color names. 


## **Background color** 
Css treats each HTML element as a box, and background- color property sets the color in the box. 

**NOTE** 
The colors of every pixel on the screen is expressed on term of red, green, and bule. 
 
### **Some terminologies**
1. **HUE**: is near to colloquial iden of a color. 
2. **Saturation**: refers to the amonut of gray in a color; max. saturation means there is no gray. 
3. **Brightness**: refers to how much black is in a color; max. brightness means there is no black 
4. **Lightness**: refers to the amount of white or black in a color; 0% represents balck lightness. 

### **Contrast** 
To make texts more readabil, so the lower the contrast the harder it is to read the text. 

# **Chapter 12** 
## **Texts**

### **Typeface Terminology**

1. **Serif**: have extra details on the ends of the main strokes of the letters. examples: Georgia,Times, and Times New Roman.

2. **Sans-Serif**: have straight ends to letters, and therefore have a much cleaner design. examples: Arial, Verdana, and Helvetica.

3. **Monospace**: Every letter in a monospace font is the same width. examples: Courier, and Courier New. 

4. **Cursive**: have joining strokes or other cursive characteristics, such as handwriting styles. examples: Comic Sans MS, and Monotype Corsiva.

5. **Fantasy**:  decorative fonts and are often used for titles. examples: Impact, and Haettenschweiler. 

**Example:** *font-family: Georgia, Times, serif;*

**NOTES**
1. font weight add emphasis; light, medium, bold, and black. 
2. font style you can use normal, italic, and oblique. 
3. font strech you can use condesned, regular, and extnended. 
4. you can use different Units of Type Size; pixels, percentages, and em. 
5. Setting font size in pixels is the best way to ensure that the type appears at the size you intendedappears at the size you intended.
6. @font-face allows to ues a font even if it is not installed in the users computer.
7. text-transform is used to determine if we wnat the text to be uppercaed, or lowercased or capitalized. 
8. text-align allows you to control the alignment of text.
9. vertical-align used with inline elements. 

# **JPEG vs PNG vs GIF**
They are the most commonly used image formats in websites and mobile applications. 

![JPEG VS PNG](!https://www.bluearcher.com/Files/Admin/blog-images/blogs-resources/jpg-vs-png-comparison-chart-resized-1.png)

## **JPEG** 
Mostly used when variation in colour and intensity is smooth, like images that contain a natural scene. is a lossy compression specification. don’t support transparency. support around 16 million colours.

## **PNG**
Used for image that needs transparency, or for images with text & objects with sharp contrast edges like logos. is a lossless image format . support transparency. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours.

## **GIF**
Usef for images that contain animations. is a lossless image format. support transparency. limited to 256 colours.

![JPEG AND PNG](https://d2dybsqaihwlah.cloudfront.net/wp-content/uploads/2017/05/24135736/pasted-image-0.png)

![jpeg vs Png](https://mlpxhq8ztvyc.i.optimole.com/QgmSm9c-8FqoPB0t/w:760/h:248/q:90/https://thrivethemes.com/wp-content/uploads/2018/05/jpg-png-filesize.png)