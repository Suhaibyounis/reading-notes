# WHAT IS AN OBJECT?

* Objects group together a set of variables and functions to create a model of a something you would recognize from the real world.
* variables and functions take on new names.

## Creating an Object:
*  **literal Notation** : the easiest and most popular way to create object.

[Creating-object](images/creating-object.jpg)


## Document Object Model
* Specifies how browsers should create a model of an **HTML page** and how **JavaScript** can access and update the contents of a web page while it is in the browser window.
* The DOM is *neither part of HTML*, *nor part of JavaScript*; it is a *separate set of rules*.
It is implemented by all major browser makers, and covers two primary areas:
1. MAKING A MODEL OF THE HTML PAGE
    * When the browser loads a web page, it creates a model of the page in memory.
    * The DOM specifies the way in which the browser should structure this model using a *DOM tree*.
    * The DOM is called an *object model* because the model (the DOM tree) is made of objects.

2. ACCESSING AND CHANGING THE HTML PAGE
    * The DOM also defines *methods and properties* to access and update each object in this model, which in turn updates what the user sees in the browser.
    * the DOM also called an *Application Programming Interface (API)*.
    * User interfaces let humans *interact with programs*; **APls** let programs (and scripts) talk to each other.
    * The *DOM* states what your script can *ask the browser about the current page*, and how to *tell the browser to update what is being shown to the user*.

## THE DOM TREE IS A MODEL OF A WEB PAGE
* As a browser loads a web page, it creates a **model of that page**.
* *The model* is called a **DOM tree**, and it is stored in the browsers' memory.
* It consists of four main types of nodes:
1. BODY OF HTML PAGE
[Body-of-the-page](images/body-of-the-page.jpg)

* THE DOCUMENT NODE
    1.  Every element, attribute, and piece of text in the HTML is represented by its own DOM node.
    2.  HTML is represented by its own *DOM node*.
    3. At the top of the tree a *document node* is added; it represents the entire page
    4. When you access any element,  attribute, or text node, you navigate to it via the *document node*. It is the starting point for all visits to the *DOM tree*.

* ELEMENT NODES
    1.  HTML elements describe the structure of an *HTML page*.
    2. The *< hl>* - *< h6>* elements describe what parts are headings; the *< p>* tags indicate where paragraphs of text start and finish; and so on.
    3. To access the DOM tree; you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to.

* Each node is an object with methods and properties.
* Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser. 

[Dom-Tree](images/dom-tree.jpg)

* ATTRIBUTE NODES
1. Attribute Nodes
The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree.
2. Attribute nodes are not children of the element that carries them; they are part of that element.
3. When you access an element, there are specific *JavaScript methods* and properties* to read or change that element's attributes.

* TEXT NODES
1. When you have accessed an element node, you can then reach the text within that element. This is stored in its own *text node*.
 2. *Text nodes* cannot have children. If an element contains text and another child element, the child element is not a child of the text node but rather a child of the containing element.

### WORKING WITH THE DOM TREE

* Accessing and updating the DOM tree involves two steps:
    1. Locate the node that represents the element you want to work with.
    2. Use its text content, child elements, and attributes.

* **STEP 1: ACCESS THE ELEMENTS**
    * Here is an overview of the methods and properties that access elements.
    * The first two columns are known as DOM queries. The last column is known as traversing the DOM.

1. SELECT AN INDIVIDUAL ELEMENT NODE
* The three common ways to select an individual element:
    * get ElementByld ()
     Uses the value of an element's id attribute
    * querySe1ector ()
    Uses a CSS selector, and returns the first matching element.
    * querySe1ector ()
    Uses a CSS selector, and returns the first matching element.

2. SELECT MULTIPLE ELEMENTS (NODELISTS)
* There are three common ways to select multiple elements.
    * getElementsByClassName()
    Selects all elements that have a specific value for their class attribute
    * getElementsByTagName()
    Selects all elements that have the specified tag name.
    * querySelectorAll()
    Uses a CSS selector to select all matching elements.

3. TRAVERSING BETWEEN ELEMENT NODES
* You can move from one element node to a related element node.
    * parentNode
    Selects the parent of the current element node (which will return just one element).
    * previousSibling / nextSibling
    Selects the previous or next sibling from the DOM tree.
    * firstChild / lastChild
    Select the first or last child of the current element.
    
* The terms elements and element nodes are used interchangeably but when people say the DOM is working with an element, it is actually working with a node that represents that element.


* **STEP 2: WORK WITH THOSE ELEMENTS**

[Work-with-Elements](images/work-with-elements.jpg)

### ACCESSING ELEMENTS

* DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.

* GROUPS OF ELEMENT NODES
    * If a method can return more than one node, it will always return a Nodelist, which is a collection of nodes.
* FASTEST ROUTE
    * Finding the quickest way to access an element within your web page will make the page seem faster and/or more responsive. This usually means evaluating the minimum number of nodes on the way to the element you want to work with.

### METHODS THAT RETURN A SINGLE ELEMENT NODE:

1. **getElementByld( 'id')**
* Selects an individual element given the value of its i d attribute .
* The HTML must have an id attribute in order for it to be selectable.

2. **querySelector('css selector')**
* Uses CSS selector syntax that would select one or more elements.
* This method returns only the first of the matching elements.

### METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):
1. **getElementsByClassName('class')**
* Selects one or more elements given the value of their class attribute.
* The HTML must have a class attribute for it to be selectable.
* This method is faster than *querySe1ectorA11()* .

2. **getElementsByTagName('tagName')
* Selects all elements on the page with the specified tag name.
* This method is faster than *querySe1ectorA11()*.

3. **querySelectorAll('css selector')
* Uses CSS selector syntax to select one or more elements and returns all of those that match.


### SELECTING ELEMENTS USING ID ATTRIBUTES

* **getElementByid()** allows you
to select a single element node
by specifying the value of its
id attribute.
* This method has one parameter:
the value of the *id attribute* on
the element you want to select.

[getElementByid](images/git-id.jpg)

### NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT.
* When a DOM method can return more than one element, it returns a *Nodelist*.
* A Nodelist is a collection of element nodes. Each node is given an index number (a number that starts at zero, just like an array).

* When a DOM query returns a Nodelist, you may want to:
    1. Select one element from the NodeList.
    2. Loop through each item in the Nodelist and perform the same statements on each of the element nodes.

* *Nodelists* look like *arrays* and are numbered like arrays, but they are not actually arrays; they are a type of object called a **collection**.

* Like any other object, a Nodelist has properties and methods, notably:
    1. The *length property* tells you how many items are in the Nodelist.
    2. The *iterm() method* returns a specific node from the Nodelist when you tell it the index number of the item that you want (in the parentheses).

### LIVE & STATIC NODELISTS
*  There are times when you will want to work with the same selection of elements several times, so the Nodelist can be stored in a variable and re-used.

* In a live **Nodelist**, when your script updates the page, the Nodelist is updated at the same time. The methods beginning *getElementsBy_return* live Node lists. They are also typically *faster to generate than static Nodelists*.

* In a **static Nodelist** when your script updates the page, the NodeList is not updated to reflect the changes made by the script.

[Node-List](images/node-list.jpg)

### SELECTING AN ELEMENT FROM A NODELIST

* There are two ways to select an element from a Nodelist:
1. The item() method.
2. array syntax.
Both require the *index number of the element* you want.

* THE item() METHOD
1. return an individual node from the
Node list.
2. You specify the index number of the element you want as a parameter of the method (inside the parentheses).

[Item-method](images/item-method.jpg)

* Array Syntax
1. faster than item() method.
2. You can access individual nodes using a square bracket syntax.

[Array-Syntax](images/array-syntax.jpg)

### SELECTING ELEMENTS USING CLASS ATTRIBUTES
* The get *ElementsByClassName()*
method allows you to select
elements whose c1ass attribute
contains a specific value.

* The method has one parameter: the class name which is given in quotes within the parentheses after the method name.

[Class-Attribute-Code](images/class-add-code.jpg)

[Class-Attribute-Result](images/class-add-result.jpg)

### SELECTING ELEMENTS BY TAG NAME
* The *getElementsByTagName()* method allows you to select elements using their tag name.

* The element name is specified as a parameter, so it is placed inside the parentheses and is contained by quote marks.

[Selecting-Element-by-tagname](images/selecting-element-by-tag.jpg)

[Selecting-Slement-by-tagname-result](images/selecting-element-by-tag-result.jpg)


### SELECTING ELEMENTS USING CSS SELECTORS
* *querySe1ector()* returns
the first element node that
matches the CSS-style selector.
*querySe1ectorA11()* returns a
Nodelist of all of the matches.

* Both methods take a CSS selector as their only parameter.
*The CSS selector syntax* offers more *flexibility and accuracy* when selecting an element than just specifying a class name or a tag name.

[Selector-CSS-Code](images/selector-css.jpg)

[Selector-CSS-Result](images/selector-css-result.jpg)


### LOOPING THROUGH A NODELIST
* If you want to apply the same
code to numerous elements, looping through a Nodelist is a powerful technique.

* It involves finding out how many items are in the Nodelist, and then setting a counter to loop through them, one-by-one.

* Each time the loop runs, the script checks that the counter is less than the total number of items in the Nodelist.

[looping-nodelist](images/looping-nodelist.jpg)

[looping-nodelist-result](images/looping-nodelist-result.jpg)

### TRAVERSING THE DOM
* When you have an element node, you can select another element in relation to it using these five properties; This is known as traversing the DOM.

1. *parentNode*
* This property finds the element node for the containing (or parent) element in the HTML.

2. *previousSibling - nextSibling*
* These properties find the previous or next sibling of a node if there are siblings.

3. *firstChild - lastChild*
* These properties find the first or last child of the current element.

[Traversing-The-Dom](images/traversing-the-dome.jpg)

### WHITESPACE NODES

* Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements.

* all of the whitespace nodes added to the DOM tree for the list example.
Each one is represented by a green square. You could strip all the whitespace out of a page before serving it to the browser. This would also make the page smaller and faster to serve/load. However, it would also make the code much harder to read.

* One of the most popular ways to address this kind of problem is to use a JavaScript library such as jQuery, which helps deal with such problems. These types of browser inconsistencies were a big factor in jQuery's popularity.

[White-Space-Nodes](images/white-space-nodes.jpg)

### PREVIOUS & NEXT SIBLING

* all spaces between the HTML elements have been removed. In order to demonstrate these properties, the second list item is selected using *getElementByld()*.

* From this element node, the *previ ousSib1ing* property will return the *first < 1i> element*, and the *next Sib1ing property* will return *the third < 1i> element*.

[Previous-Next-Sibling](images/previous-next-sibling.jpg)















