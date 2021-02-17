# **Chapter 4**

## **Links** 

### **Creating links between pages:**
- Links allow the user to move from one place to another, there is different types of links we can add: 
1. **Absolute links:**
    - They are like a shorthand version of absolute URLs. 
    - Links to allow the user to move to a new browser.
    - Links to allow the user to move from one website to another.
    - Links to allow the user to start up an email.

2. **Relative links:** 
    - Links to allow the user to move from one page to another in the same website.
    - Links to allow the user to move from one part of the page to another.

Links are created by using the "< a >" element, you specify which page you want to link by using "href" attribute.

***for example*** 


![Example 1](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRx5mibponwJR59Rar_F-qKQVhuq9PfCEGLhw&usqp=CAU) 

- In the example above you can see how links are added, note that the "text" in the example is to be filled with the text to be shown to the user. 

- To link one part of a page to another part, the part you want to link must have a an id attribute that identifies it. 

![Example 3](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQBiwq9kRbfLBrOjXWFf79TyP-B1jZTRh8GgQ&usqp=CAU)


# **Chapter 15**

## **Layout**
Css deals with each HTML as an indivial box. The box will be either a block-level or an inline-level. 

### ***CSS positioning schemes types***

Normal flow | Relative Positioning |Absolute positioning
------------|----------------------|--------------------
the default layout, Every block-level element appears on a new line.is not positioned in any special way; it is always positioned according to the normal flow of the page. | is positioned relative to its normal position. Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. | This positions the element in relation to its containing element. It is taken out of normal flow, Absolutely positioned elements move as users scroll up and down the page.


**Fixed vs floating elements:** 
* fixed elements: it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element. 
* floating elements: allows you to take that element out of normal flow and position it to the far left or right of a containing box. 

**NOTE**
When elements are positioned, they can overlap other elements. The z-index property specifies which element should be placed in front of, or behind, the others. 

 **Layout**

-	**The traditional layout:** it uses < div> element, It normally consists of a: 
1.	Header: containing a logo.
2.	Body: containing posts.
3.	Sidebar.

-	**Newer layouts:**: uses < nav>, < article> elements more. 

## **Some elements meaning**

1.	< nav> : used to contain the main navigational blocks.
2.	< article> : a container for any section. 
3.	< aside> : when it is used in an < article> element, contains related but not essential, outside  an < article> element it acts as a container. 
4.	< section> : it relates content together 
5.	< hgroup> : heading group, to group a set of one or more heading, so they are treated as a single head. 
6.	< figures> : < figures> < figcaption>, it is used when the content references the element and not something integral to the page flow. 

### **Screen sizes** 
each user have a different screen size depending on the kind of device the user uses, so the design needs to fit in a suitable way on a range of different sized screens. 

**Fixed width layout** do not change size as the user increases or decreases the size of their browser window.

![fixed](https://image.slidesharecdn.com/csslayouttechniques-130623051248-phpapp02/95/css-layout-techniques-24-638.jpg?cb=1371964476)

**Liquid Layouts** stretch and contract as the user increases or decreases the size of their browser window They tend to use percentages. 
![liquid](https://image.slidesharecdn.com/csslayouttechniques-130623051248-phpapp02/95/css-layout-techniques-31-638.jpg?cb=1371964476)


# **Chapter 3 from js book**

## **The Dom Tree**
The browser creats a model of a page when the page is loaded, this model is called a **DOM tree**, it stored a memory

**The model consists of four main types of nodes:**
1. THE DOCUMENT NODE: represents the entire page
2. ELEMENT NODES
3. ATTRIBUTE NODES
4. TEXT NODES 

![DOM TREE](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png)

# **Pair programming** 
is when two developers share a single workstation to ineratively tackle a coding task together. involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard.The Navigator uses their words to guide the Driver but does not provide any direct input to the computer.

### **Pair programming adavantages:** 
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness

