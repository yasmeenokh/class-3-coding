# Responsive Web Design (RWD)

**RWD**: means building a website that is suitably displayed on all kind of devices, ie on every screen size. 

![rwd](http://vivid360.com.ng/wp-content/uploads/2016/03/responsive-web-design-vivid360-design.jpg)

### Differentiating between terminologies: 

Responsive | to react quickly and positively to any change.
-----------|-----------------------------------
Adaptive   | to be easily modified for a new purpose or situation, such as change.
Mobile     | to build a separate website commonly on a new domain solely for mobile users.

## Flexible Layouts
building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units. 

## Media Queries
provide the ability to specify different styles for individual browser and device circumstances.

![mq](https://www.emailonacid.com/images/blog_images/Emailology/2017/EOA_MediaQueriesNEW_Blog.jpg)

Ways to use media queries:
1. @media 
2. @import 

### Logical Operators in Media Queries

![logical](https://1.bp.blogspot.com/-YH9B5kBZAj8/Xx5v118EAWI/AAAAAAAAEDk/3IY-AOoz0kI6ZaQjmE6EGb-u5FNfRBczwCLcBGAsYHQ/w625-h110/media-types.png)

here are three different logical operators available for use within media queries, including and, not, and only.

* And : allows an extra condition to be added, making sure that a browser or devices does both.
* Not : negates the query, specifying any query but the one identified.
* Only : hiding the styles from devices or browsers that don’t support media queries.

![and/not/only](https://i.stack.imgur.com/mMvC7.png)

### Media Features
1. Height & Width.
2. Orientation.
3. Aspect Ratio.
4. Resolution.

### Mobile First
includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

### Viewport
Using the viewport meta tag with either the height or width values will define the height or width of the viewport respectively. 

## Flexible Media
Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

# All About Floats
There are four valid values for the float property. Left and Right float elements those directions respectively. None (the default) ensures the element will not float, and Inherit which will assume the float value from that elements parent element.

**Uses:**
* Wrapping text around images. 
* create the entire web layouts. However they are more helpful in smaller instances; ie smaller sections. 

**Clear Property** 
When an element has the clear property it will not move up adjacent to the float like the float desires, but will move itself down past the float. 

+ Clear values: **both**, left, right, inherit.

**NOTES** 
* Be aware that floats can affect their parent element; so if the parent element contained nth but the floats, it's would collapse to nothing. 
* This can be fixed by clearing the float after the floated element and before the close of the container. 

### Ways to clear floats 
1. The Empty Div Method 
2. The Overflow Method
3. The Easy Clearing Method: using  a pseudo selector **:after**. 

## Floats disadvantages
1. Push-down: when an element inside a float, but wider than the float itself. This can be fixed by using overFlow: hidden. 

2. Double Margin Bug: this can be fixed by using display: inline. 

3. 3px Jog: when text that is up next to a floated element is kicked away by 3px. This can be fixed by setting a width or height on the affected text. 

4. Bottom Margin Bug: when if a floated parent has floated children inside it, bottom margin on those children is ignored by the parent. This can be fixed by using bottom padding on the parent instead. 

# Grids 
you can define grids in css, but use grid or flexbox.

# CSS Floats Explained By Riding An Escalator

* an analogy on css floats based on how people either stand to the left, to the right, and a 'passing lane'
and uses same analogy for clearing floats

# SMACSS 

SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS. 