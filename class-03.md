# **Chapter 3**
## **Lists in html**

**Types of lists** 

ordered list | unorderd list | definition list 
-------------|---------------|----------------
a numbered list | uses bullet points | a set of terms a long with their defentions 
-------------|------------|-------------
< ol > </ ol > tags and then each item is list in < li > </ li> tags| < ul> </ ul> tags and then each item is list in < li > </ li> tags| < dl> </ dl > tags and then < dt > </ dt > to list each term, and < dd> </dd> to contain the definition. 


# **Chapter 13**
## **Boxes** 
- since css deals with the html page as a set of box, so it is better to divide your page into boxes. 

**Edits you can do to each box:** 

* you can change it's width and hight, we do so by using pixels, percentages, or
ems.
* min-width/ max width and min-height/ max-height are used to ensure that the content of the page is shown in the suitable way in all different sizes of devices. 
* overflow is used when the content of a box is bigger than the box, this property can hide any extra content that doesn't fit, or add a scrollbar.

### To control the appearance of a box: 
1. borders: separates the edge of one box from the other.
2. margins: to create a gap between the borders the boxes.
3. paddings: the space between the border of a box and any other content in it.

**Note** 
* you can play with border's style, color and width. 
* padding make text easier to read, and it is normally specified using px.

### **Display:**
turn an inline element into a block-level element or the other way around.

![dispaly](https://bloc-global-assets.s3.amazonaws.com/images-design/jottly/css/css-display.png)

# **Chapter 2 from js**
## **Arrays**
Stores a list of values related to each other, used when one doesn't know how many items a list will contain. 

**Creating an array:** 
We still use the var keyword, for example 
var type= ["number" , "string" , "boleen"]

**NOTE**
Values in arrays are delt with as if they are in a numbered list. 
It is important to know that numbering starts at zero not one.
Each item is automatically given a number known as index. 

# **Chapter 4**
## **If else statement**

![if stat.](https://cdn.javascripttutorial.net/wp-content/uploads/2016/08/JavaScript-if-else-statment.png)
 
If determines wether a condition is true or not, if true the first code block will run, if not the second code block will run.

![syntax](https://cdn.programiz.com/sites/tutorial2program/files/js-if-else-statement.png)

## **Switch statement**

they are used to perform different actions based on different conditions. Use switch to select one of many blocks of code to be executed. it is normally used when we have long if/else statements. 

1[switch](https://slideplayer.com/slide/6322656/21/images/2/The+JavaScript+Switch+Statement.jpg)

**NOTE**
**Type Coercion in js** refers to the automatic or implicit conversion of values from one type to another. 

## **Loops**

Checks a condition if true a code block will run. It repeats until the condition return false 



### **Types of loops:** 

**For** | **While**| **Do While** 

--------|----------|------------

To run a code a specific number of times, the condition is normally a counter. | If you don't know how many times you want to run the code, the code will continue to loop as long as the condition is true. | It will run the condition at least once even if the condition is false. 

### **For condition** 

![for condition](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/for-Statement.png)



## **While condition**

![while condition](https://www.tutorialspoint.com/javascript/images/while_loop.jpg)



## **Do While condition** 

![do while](https://media.geeksforgeeks.org/wp-content/uploads/20191118154342/do-while-Loop-GeeksforGeeks2.jpg)






