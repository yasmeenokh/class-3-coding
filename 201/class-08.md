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



