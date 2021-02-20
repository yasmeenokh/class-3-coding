# **Understanding The Problem Domain**
understanding the problem domain helps programmers to write the code much faster and more efficiently. a programmer should always understand the purpose and how something should, in order to be able to code correctly. 

- It is very difficult to solve a problem before you know the question."

**Understanding the problem domain is the hardest part of programming** 

## **To make programming easer:**
1. Make the problem domain easier:
cutting out cases and narrowing your focus to a particular part of the problem.

2. Get better at understanding the problem domain:
make sure you understand a problem inside and out before you try and solve it with code. before starting with coding you should set with your client and fully understand the problem domain. 

**Marketing and branding yourself is very important, and it should be done efficiently; this will highly increase one's opportunities. 

# **Chapter 3** 

## **Object Literals**
**Objects group together a set of variables and functions to create a model** variables are called properties, and functions are called methods. each property has a key(name) and a value.

**NOTES** 
Dot notation is used to access a property or a methods in an object. Methods can also be invoked using dot and bracket notation as well. 

![dot notation](https://miro.medium.com/max/797/1*4ArCZQYVIH3SKAY0JzYpng.png). 

# **Chapter 5** 
## **Document Object Model** 
**Document Object Model** (DOM), specifies how a browser should create an HTML model and how can JS access it whit it is in the browser window. 

**The Dom Tree**
The browser creates a model of a page when the page is loaded, this model is called a **DOM tree**, it stored a memory

**The model consists of four main types of nodes:**
1. THE DOCUMENT NODE: represents the entire page
2. ELEMENT NODES
3. ATTRIBUTE NODES
4. TEXT NODES 

![DOM TREE](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png)

**Accessing the elements in a DOM**
![dom access](https://miro.medium.com/max/734/1*ZUa-HtPgJNKl67EFpVp2Kg.png)

### **DOM queries** 
we find elements in a DOM tree using DOM queries. you access an element within the DOM tree for example:
1. using the id attribute: getElementById().
2. using Css selector: querySelector().
3. Nodelists : getElementByClassName().
4. Nodelists : getElementByTagName().
5. Nodelists : querySelectorAll(). 

**NOTES** 
1. length property tells you how many items are in a nodelist.
2. item() returns a specific node form a nodelist, using the index number of that item. we can use [] same as done with arrays.

### **Traversing the DOM**
selecting an element in relation to an element in the node. 

**This is done by:**
* parentNode
* previouseSibling/ nextSibling 
* firstChild/ lastChild

### **Updating element content**
* The innerText property returns just the text, without spacing and inner element tags ( avoid it's use).
* The innerHTML property returns the text, including all spacing and inner element tags.
* The textContent property returns the text with spacing, but without inner element tags.
* Dom manipulation also allows you to add add new content to the page.

![inner](https://www.programmersought.com/images/260/da04da8a24cf496945c138a9e7af6a0c.gif)

**nodeValue** property allows you to edit or get the content of a node.

**Dom manipulation**
to create a new element:
1. createElement()
2. createTextNode()
3. appendChild()

**document.write()** | **element.innerHTML** | **DOM MANIPULATION**  
---------------------|-----------------------|--------------------
easy way to add content however it only adds content when the page is loaded, otherwise it will overwrite the page or not add the content. | update the entire content of any element (including markup) as a string, it uses less code, and faster than don manipulation. However it is not to be used to content added by the user, hard elemet isolation for single elements in a large DOM fragment.| it works best for changing one element with many siblings, allows a script to add elements incrementally. However slower that innerHTML if few changes are made, uses more code. 

### **Cross-Site Scripting Attacks**
when you add content using innerHTML this can cause Cross-Site Scripting Attacks, an attacker could gain access to the users' accounts.

### **Attribute nodes**

![attribute](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/Attribute-Nodes-in-JavaScript-DOM.jpg)

*Creating attributes*

![creating](https://www.encodedna.com/javascript/create-dynamic-ul-and-li-using-javascript.png)













