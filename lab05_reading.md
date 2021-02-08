# **Reading 05:**

## **How forms are work** 

A form is filled by a user with a certain information and then submitted to the server. The server processes the information using a programming language, it can also be saved in a data base. The browser then sends a new page with a massage based on the information received. 

**NOTE**

To differentiate between different types of input data, information is sent to the browser using “name/value” in pair. 

## **Form Structure** 

**Form** element is used, it uses an **action** attribute and may have a **method** and **id** attribute. 

**Action**  | **method**
-----------------|---------------
It carries the URL for the server that will receive the information submitted. | Is how the form is sent, it can be sent by get or post.


***The differance between get and post***

**Get** | **Post**
------------|-------------   
Adds the form value to the URL end specified in the action attribute. Used for short forms, or when data is retrieved from the web.| values are set in HTTP headers. Used to upload files or when forms are long, or contain a sensitive data, or add, delete information from a data form. 

**Id:** is used to differentiate a form from other elements in the page.  
###  **Checkbox:** 

![check box example](checkbox.jpg)

Allows the user to select one or more option, **name** attribute is added and sends selected values to the server. 

**Value** indicate the value sent to the server if a box is checked. A value can be checked by defaulf by adding checked attribute. 

### **Drop down list:**

![drop down example](dropdownlist.jpg)

Allows the user to select one option from a drop down list. Select element is used to create a drop down list. Option element is used to specify an option selected by the user. It uses a closing tag, and a **value** attribute to indicate the value sent to the server. 

**NOTE** 

For short list **radio** is better to be used, **drop down list** is better to be used for long lists.

![radio example](radioinhtml.jpg)

## **Labels**
Each form control should have its own label element.

1. **For** attribute to state which form control the label belongs to. 

**Best places to place labels:**

2. Above or to the left: text inputs, text areas, select box, file uploads. 

 3. To the right: individual checkbox, radio buttons. 
  
  ## **Grouping form element 
  
  By using **fieldset** element; important for long forms. **Legend** element is used to identify the     purpose of the form group. 

## **Form validation:**

To make sure a field is filled by the user, this reduces the amount of the work done by the server. It also enables the users to identify problems with the form faster. 

**NOTE** 

**Input** is used to determine the type the texts inserted.




 


