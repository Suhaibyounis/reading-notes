# HTML Links, CSS Layout, JS Functions

## Links
* Creating links between pages
* Linking to other sites
* Email links

* Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

## Writing Links
Links are created using the < a> element. Users can click on anything between the opening < a> tag and the closing < /a> tag. You specify which page you want to link to using the href attribute.

[Writing-Links](images/writing-links.jpg)

* The text between the opening < a> tag and closing < /a> tag is known as **link text**.

## Linking to Other Sites
* Links are created using the <a> element which has an attribute called **href**.

* When you link to a different website, the value of the href attribute will be the full web address for the site, which is known as an **absolute URL**.

* Browsers show links in **blue** with an **underline** by default.

[Links](images/links/jpg)

## Linking to Other Pages on the Same Site
* When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a **relative URL**.
* If all the pages of the site are in the same folder, then the value of the **href attribute is just the name of the file**.

[linking-to-other-page](image/linking-to-other-page.jpg)

## Directory Structure

*On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a **new folder**.
* **Folders** on a website are sometimes referred to as **directories**.

1. Structure
* The diagram shows the directory structure for a fictional entertainment listings website called **ExampleArts**.

* The top-level folder is known as **the Root folder**. (In this example, the root folder is called **examplearts**.) The root folder contains all of the other files and folders for a website.

* Each section of the site is placed in a separate folder; this helps organize the files.

2. Relationships
* The Relationship between *files* and *folders* on a website is described using the same terminology as a **family tree**.
* The examplearts folder is a parent of the movies, music and theater folders. And the the movies, music and theater folders are children of the examplearts folder.

3. Home pages
* The main homepage of a site written in HTML (and the homepages of each section in a child folder) is called index.html.

* Web servers are usually set up to return the index.html file if no file name is specified.

* Therefore, if you enter *examplearts.com* it will return **examplearts.com/index.html**, and *examplearts.com/music* will return **examplearts.com/music/index.html**.

[dir.structure](images/dir-structure.jpg)

4. Relative URLS

* Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.

* When you are linking to a page on your own website, you do not need to specify **the domain name**. You can use **relative URLs** which are a shorthand way to tell the browser where a page is in relation to the current page.

[Relative-URL](images/relative-url/jpg)

5. Email Links 
* To create a link that starts up the user's email program and addresses an email to a specified email address, you use the < a> element.

[Email-Link](images/email-link.jpg)

6. Opening Links in a New Window
* **target** : If you want a link to open in a new window, you can use the **target attribute** on the opening < a> tag. The value of this attribute should be _blank.

7. Linking to a Specific Part of the Same Page
* At the top of a long page you might want to add a list of contents that links to the corresponding sections lower down. Or you might want to add a link from part way down the page back to the top of it to save users from having to scroll back to the top.

[Linking-inside-the-Page](images/linking-inside.jpg)

8. Linking to a Specific Part of Another Page

[Linking-with-other-page](images/linking-with-other-page.jpg)

***

# Layouts
* Controlling the position of elements
* Creating site layouts
* Designing for different sized screens

## we are going to look at how to control where each element sits on a page and how to create attractive page layouts.

* Explore different ways to position e ●● lements using normal flow, relative positioning, absolute positioning and floats.
* Discover how various devices have different screen sizes and resolution, and how this affects the design process.
* Learn the difference between fixed width and liquid layouts, and how they are created.
* Find out how designers use grids to make their page
designs look more professional.

## Key Concepts in Positioning Elements
1. Building Blocks
* CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

* Block-level elements 
start on a new line Examples include:
< h1> < p> < ul> < li>

[Block-Level](images/block-level.jpg)

* Inline elements
flow in between surrounding text Examples include:
< img> < b> < i>

[Inline-Element](images/inline-element.jpg)

* Containing Elements
If **one block-level element** sits inside another block-level element then the outer box is known as the **containing or parent element**.

[containg-element](images/containg-element.jpg)

* The orange lines in this diagram represent **< div>** elements. The header (containing the logo and navigation) are in one **< div>** element, the main content of the page is in another, and the footer is in a third.
* The **< body>** element is the containing element for these three **< div>** elements. 
* The second **< div>** element is the containing element for two paragraphs of Latin text and images (represented by crossed squares).

## Controlling the Position of Elements

**CSS** has the following **positioning schemes** that allow you to control the layout of a page: *normal flow*, *relative positioning*, and *absolute positioning*. You specify the **positioning scheme** using the **position property** in CSS. You can also **float elements** using the **float property**.

[Positioning-schemes](images/positioning-schemes.jpg)

* To indicate where a box should be positioned, you may also need to use **box offset** properties to tell the browser how far from the top or bottom and left or right it should be placed.

[Box-Offset](images/box-offset.jpg)

## Normal Flow
* In normal flow, each block-level element sits on top of the next one. the syntax would be:

    * position: static;
    There is no specified a width property for the heading element, so you can see how it stretches the width of the entire browser window by default.

    * position:relative
    Relative positioning moves an element in relation to where it would have been in normal flow.

    * position:absolute
    When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page.

    * position:fixed
    Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.
* When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page.

## OverLapping Elements
* z-index
If you want to control which element sits on top, you can use the z-index property. Its value is a number, and the higher the number the closer that element is to the front.

## Floating Elements
* float
    * The float property allows you to take an element inormal flow and place it as far to the left or right of the containing element as possible.
    * Anything else that sits inside the containing element will flow around the element that is floated.



## Using Float to place Elements side-by-side.

* A lot of layouts place boxes next to each other. The float property is commonly used to achieve this.
* When elements are floated, the height of the boxes can affect where the following elements sit.

## Clearing Floats
* The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:

1. left: 
The left-hand side of the box should not touch any other elements appearing in the same containing element.
2. right:
The right-hand side of the box will not touch elements appearing in the same containing element.
3. both:
Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.
4. none:
Elements can touch either side.

## Parents of Floated Elements: 
1. Problem
* If a containing element only contains floated elements, some browsers will treat

2. Solution
* A CSS rule would be applied to this additional element setting the clear property to have a value of both. But this meant that an extra element was added to the HTML just to fix the height of the containing element.

*The pure CSS solution adds two CSS rules to the containing element (in this example the <div> element):
1. The overflow property is given a value auto.
2. The width property is set to 100%.

## Creating Multi-Column Layouts with Floats
* Many web pages use multiple columns in their design. This is achieved by using a < div> element to represent each column.
* Three CSS properties are used to position the columns next to each other:
1. width
    * This sets the width of the columns.
2. float
    * This positions the columns next to each other.
3. margin
    * This creates a gap between the columns.


## Screen Sizes
* Different visitors to your site will have different sized screens that show different amounts of  nformation, so your design needs to be able to work on a range of different sized screens.

## Screen Resolution
* Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

## Page Sizes
* Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide.

## Fixed Width Layouts
* Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

* **Advantages**
    * Pixel values are accurate at controlling size and positioning of elements.
    * The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
    * You can control the lengths of lines of text regardless of the size of the user's window.
    * The size of an image will always remain the same relative to the rest of the page.

* **Disadvantages**
    * You can end up with big gaps around the edge of a page.
    * If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
    * If a user increases font sizes, text might not fit into the allotted spaces.
    * The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.
    * The page will often take up more vertical space than a liquid layout with the same content.

## Liquid Layouts
* Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

* **Advantages**
    * Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.
    * If the user has a small window, the page can contract to fit it without the user having to scroll to the side.
    * The design is tolerant of users setting font sizes larger than the designer intended (because the page can stretch).

* **Disadvantages**
    * If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.
    * If the user has a wide window, lines of text can become very long, which makes them harder to read.
    * If the user has a very narrow window, words may be squashed and you can end up with few words on each line.
    * If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the window smaller) the image can overflow over the text.

## A Fixed Width Layout
* To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too).

## A Liquid Layout
* The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen.

## Layout Grids

* Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements.
* Many designers use a grid structure to help them position items on a page, and the same is true for web designers.

* Grids set consistent proportions and spaces between items which helps to create a professional looking design.

* While a grid might seem like a restriction, in actual fact it:
1. Creates a continuity between different pages which may use different designs 

2. Helps users predict where to find information on various pages.

3. Makes it easier to add new content to the site in a consistent way

4. Helps people collaborate on the design of a site in a consistent way.

[Grid](images/grid.jpg)


## CSS Frameworks
* Aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on.

* **ADVANTAGES**
1. They save you from repeatedly writing code for the same tasks.
2. They will have been tested across different browser versions (which helps avoid browser bugs).

* **DISADVANTAGES**
1. They often require that you use class names in your HTML code that only control the presentation of the page (rather than describe its content).
2. In order to satisfy a wide variety of needs, they often contain more code than you need for your particular web page (commonly referred to as code “bloat”).

There are several gridbased CSS frameworks available online, such as those at:
[960](https://960.gs/)
[Blue=Prints](http://blueprintcss.org/)
[Lessframework](https://lessframework.com/)

## CSS Frameworks provide rules for common tasks.
## You can include multiple CSS files in one page.

***
***
***
# Functions, Methods, and Objects

## FUNCTIONS
* ***Functions*** used to group a series of statements together to perform a specific task.

* **Functions** offer a way to store the steps needed to achieve the task.

* **Calling the Function**

* **Parameters**: Pieces of information passed to a function.

### [Parameters](Parameters.jpg)

* **Return value**: The expected answer that function will provide you with answers.

### [return](return.png)

* **updatemessage** ; we can update the content of the page by document.getElementbyid

[html](images/html1.jpg)

[javascribt](images/javascribt1.jpg)

[result](images/result.jpg)

***

## Declaring a Function
Its giving the function name and then write the statements needed to achieve its task inside the curky braces.

* Declaring a function using the **function** keyword.
* Giving the function a **name** followed by parentheses.
* The **statement** that perform the task sit in a code block

[Declaring-Function](declaringfunction.jpg)

***

**Calling the Function**: It's asking the fuction to perform its tadk, and the name shoul describe the task which it's performing.

### [Calling_Function](Calling function.gif)

* to run the code in the function, you ude the function name followed by **parentheses**.

* You can call the same function as many times as you want within the same JavaScript file.

***

## Declaring a Function that need Information

* Sometimes a function needs specific information to perform its task.

* Sometimes you declare the function you give it parameters.

* Inside the function, the parameters act like variables.

[function-declaring](function-declaring.jpg)

## Calling function that has parameters, you specify the values it should use in the parentheses that follow its name, these values called **Arguments**

* Arguments as **Values**
getArea(3, 5);

* Arguments as **Variables**
wallwidth = 3;
wallhright = 5;
getArea(wallwidtg, wallheight);

### **Parameters** vs **Arguments**
* Parameters; when the function is declared, you will see the words **width**and **height** used. inside the curly braces of the fubction, those words act like **Variables**.

* Arguments; in above you can see that the **getArea()** function in being called and the code specifies real numbers that will be used to perform the calculation, these values which passed into the code are called **Arguments**.

## Getting a Single Value out of a Function
* some functions return information to the code that called them.

[single-value](singlevalue.jpg)















