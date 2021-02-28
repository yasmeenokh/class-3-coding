# **ANIMATED CHARTS WITH CHART.JS** 
### **Drawing a line chart:** 
first we start with importing the js in our HTML, then creat a canvas element in the html, then we start a script to retrive the context of the canvas, and creat the data.

![line](https://www.excel-easy.com/smi/examples/line-chart.png)

### **Drawing a pie chart** 
we add the option pie to our script, creat the data, all we have to is to add a value and a color for each section. 

![pie](https://d2mvzyuse3lwjc.cloudfront.net/doc/en/UserGuide/images/2D_B_and_W_Pie_Chart/2D_B_W_Pie_Chart_1.png?v=83139)

### **Drawing a bar chart** 
same as before but we choose bar value, add data, however time we’ve chosen to use RGBA to specify our colors which allows us to add transparency.

![bar](https://res.cloudinary.com/practicaldev/image/fetch/s--04Uz3pU---/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/pdg4eqlpz1hjjfwcdsxj.png)

# **Basic usage of canvas**
<canvas id="" width="" height=""> </canvas>
the width and height value are optional,The element can be sized arbitrarily by CSS. 
getContext(); method that takes one parameter; is used to obtain the rendering context and its drawing functions.

# **Drawing shapes with canvas**

## **The grid**
Normally 1 unit in the grid corresponds to 1 pixel on the canvas

### **Drawing rectangles**
 < canvas > only supports two primitive shapes: rectangles and paths. 

**Functions to draw a rectangle:**
1. fillRect(x, y, width, height) this draws a filled rectangle.
2. strokeRect(x, y, width, height) this draws a rectangular outline.
3. clearRect(x, y, width, height) this clears the specified rectangular area, making it fully transparent.

### **Drawing paths**
A path is a list of points, connected by segments of lines that can be of different shapes. 

**Steps to draw a path**
1. beginPath()
2. Path methods
3. closePath()
4. stroke()
5. fill()

**NOTE**
* moveTo(x, y) Moves the pen to the coordinates specified by x and y.
* For drawing straight lines, use the lineTo() method; lineTo(x, y). 
* to draw a circle, we use the arc() or arcTo() methods; arc(x, y, radius, startAngle, endAngle, anticlockwise).

## **Path2D objects**
lets you cache or record these drawing commands. You are able to play back your paths quickly.

# **Applying styles and colors**
1. fillStyle = color; Sets the style used when filling shapes.
2. strokeStyle = color; Sets the style for shapes' outlines.

### **Transparency**
globalAlpha = transparencyValue
Applies the specified transparency value to all future shapes drawn on the canvas. 
### **Gradients**
1. createLinearGradient(x1, y1, x2, y2)
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
2. createRadialGradient(x1, y1, r1, x2, y2, r2) Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.
3. createConicGradient(angle, x, y) Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

# **Drawing text** 
1. fillText(text, x, y [, maxWidth]) Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
2. strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
