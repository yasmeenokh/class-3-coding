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
