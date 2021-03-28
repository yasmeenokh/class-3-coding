# JQUERY 
With JQUERY we can perform tasks in a simpler way:
* **Select Elements:** we can find elements using CSS-style selectors.
* **Perform Tasks**
* **Handle Events**

![adva](https://4.bp.blogspot.com/-Q5FMiE1WTAY/XNrQpooTO7I/AAAAAAAABbc/sA9zb8eEcGQA9hJcdFhsslbuxc-P_UKFgCLcBGAs/s1600/features-of-jquery.png)

**NOTE:**
In order to use jQuery, the first thing you need to do is include the jQuery script in your page. You can see that it is included before the closing </ body> tag.

### WHY USE JQUERY?
* Is much faster at selecting elements.
* Can be a lot more accurate about which elements
to select.
* Often require a lot less code than older DOM
methods.
* Are already used by most front-end developers.
* Common tasks in less code. 
### Get and Set Data:
- Get: when a JQUERY selection hold more than one element, when we get the element it will only retrieve information from the first one. The .html() and  .text() methods both retrieve and update the content.

- Set Information: when a JQUERY selection hold more than one element, and a method is used to add data it will be added to all elements. The .append () method lets you add content to the page

### Some function with JQUERY:
1. Load event: has been replaced with .on(), the on event is fired with the whole page is loaded.

2. .ready(): checks if the browser supports the DOMContentLoaded event. It doesn't however wait for the assets to finish loading.

### Updating Data:
1. .html()
2. .text()
3. .replaceWith()
4. .remove()

### Inserting Elements
1. .before()
2. .after()
3. .prepend()
4. .append()

### GETTING AND SETTING ATTRIBUTE VALUES: 
1. .att()
2. .removeAtt()
3. .addClass()
4. .removeClass()

*** We can also get and set CSS properties using .css() method. ***

### jQuery allows you to recreate the functionality of a loop on a selection of elements 
* .each() : Allows you to perform one or more statements on each of the items in the selection of elements that is returned by a selector - rather like a loop in JavaScript.

* this : you can access the current element using the this keyword.

## EVENT METHODS 
The .on() method is used to handle all events.

![EVent](https://image.slidesharecdn.com/jquerybesic-150328142443-conversion-gate01/95/jquery-besic-17-638.jpg?cb=1427552893)

### Delegating events: 

![delegating](https://images.slideplayer.com/12/3493806/slides/slide_20.jpg)

# Ways to include JQUERY in the page: 
1. From a CDN: It starts with a < script> tag that tries to load the jQuery file from the CDN. But note that the URL for the script starts with two forward slashes (not http:). This is often followed by a second < script> tag that contains a logical operator, which checks to see if jQuery has loaded.

**NOTE** 
The best place to put our JQUERY script is before the closing body tag; because the the script is not blocking other things from downloading, and the DOM has already been loaded. 

# Pair Programming
**ADVANTAGES** 
1. Greater efficiency.
2. Engaged collaboration.
3. Learning from fellow students.
4. Social skills.
5. Job interview readiness.
6. Work environment readiness.

# Attribute Nodes
With node elements, we can use other properties and methods on that element. 

![methods](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/08/Attribute-Nodes-in-JavaScript-DOM.jpg)

# Repeating actions for an entire nodelist
You can loop through each node in the collection and apply the same code to each one. 




