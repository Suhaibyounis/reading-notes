# HTML Tables; JS Constructor Functions

## Table
* WE will learn how to:
1. Use the four key elements for creating tables.
2. Represent complex data using tables.
3. Add captions to tables.

## Definition of Table :
* A table represents information in a grid format.
Examples of tables include financial reports, TV schedules, and sports results.

* Grids allow us to understand complex data by referencing information on two axes.

* Each block in the grid is referred to as a *table cell*. In HTML a table is written out row by row.
[Table](images/table.jpg)

## Basic Table Structure

###
    * The < table> element is used to create a table. The contents of the table are written out row by row.

* **< tr>**
    * You indicate the start of each row using the opening < tr> tag. (The tr stands for table row.)
    * It is followed by one or more < td> elements (one for each cell in that row). 
    * At the end of the row you use a closing < /tr> tag.
* **< td>**
    * Each cell of a table is represented using a < td> element. (The td stands for table data.)

[Createing-Table](images/table-create.jpg)


### Table Headings
* **< th>**
    * The **< th>** element is used just like the < td> element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)

    * Even if a cell has no content, you should still use a < td> or < th> element to represent the presence of an empty cell otherwise the table will not render correctly.

    * Browsers usually display the content of a **<th>** element in **bold** and in **the middle of the cell**.

[Table-Cells](images/table-cells.jpg)

### Spanning ColumnS

* The **colspan** attribute can be used on a < th> or < td> element and indicates how many columns that cell should run across.

[Table-Spanning](images/table-spanning.jpg)

### Spanning Rows

* The **rowspan** attribute can be used on a < th> or < td> element to indicate how many rows a cell should span down the table.

[Table-Row-Spanning](images/table-rows-spanning.jpg)

### Long Tables

* There are three elements that help distinguish between the main content of the table and the first and last rows.

    * use screen readers
    * allow you to style these sections in a different manner than the rest of the table.

1. **< thead>**
The headings of the table should sit inside the < thead> element.
2. **< tbody>**
The body should sit inside the < tbody> element.
3. **< tfoot>**
The footer belongs inside the < tfoot> element.

[Table-Long](images/table-long.jpg)

[Table-Long-result](images/table-long-result.jpg)

### Old Code

1. Width & Spacing

* The **width attribute** was used on the opening *< table> tag* to indicate how wide that table should be and on some opening *< th> and < td> tags* to specify the *width* of individual cells.
* The value of this attribute is the width of the table or cell in pixels.

* The columns in a table need to form a straight line, so you often only see the width attribute on the first row.

* The opening *< table> tag* also use the cellpadding attribute to add space inside each cell of the table, and the cellspacing attribute to create space between each cell of the table.

[Table-Width-and-Spacing](images/table-width.jpg)

2. Border & Background

* The **border attribute** was used on both the *< table> and < td>* elements to indicate *the width of the border in pixels*.

* The **bgcolor** attribute was used to indicate *background colors* of either the entire table or individual table cells.

[Table-Background](images/table-bg.jpg)

***
***
 # Functions, Methods, and Objects

 ### Creating an Object: Construction Notation

 * The new Keyword and the Object constructor create a blank object.
 * You can then add Proporties and methods to the object.

 [Object-Create](images/object-create.jpg)

### Updating and Object

* To update the value of Proporties, use *dot notation or square brackets*.
* To delete a property, use the *delete* keyword.

[Object-Update](images/object-update.jpg)


### CREATING OBJECTS USING CONSTRUCTOR SYNTAX

* Why we might want to create multiple objects on the same page?

* **A constructor function** defines a template for the hotels. Next, two different instances of this type of hotel object are created. The first represents a hotel called Quay and the second a hotel called Park.

* Having created instances of these objects, you can then access their *properties and methods* using the same *dot notation* that you use with all other objects.

[Object-Counstruction](images/object-construction.jpg)


### ADDING AND REMOVING PROPERTIES

* We can do this using the **dot notation**.

[Object-add-and-remove](images/object-add-and-remove.jpg)

[Object-Create-Recap](images/object-create-recap.jpg)

### This 

* The keyword **this** is commonly used inside **functions and objects**.
* Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.

1. A FUNCTION IN GLOBAL SCOPE.
* When a function is created at the top level of a script (that is, not inside another object or function), then it is in the global scope or global context.

 function windowSize() {
    var width= this.innerWidth;
    var height = this.innerHeight;
    return [height, width];
 }

2. GLOBAL VARIABLES

* All global variables also become properties of the window object. so when a function is in the global context, you can access global variables using the window object, as well as its other properties.

***
var width = 600 ;
var shape = {width: 300};
var showWidth-= function(){
document.write(this.width) ;
};
***

3. A METHOD OF AN OBJECT

* When a function is defined inside an object, it becomes a method. In a method, this refers to the
containing object.

var shape = {
    width : 600,
    height : 400,
    getArea: function(){
        return this.width * this.height;
    }

};

4. FUNCTION EXPRESSION AS METHOD

* If a named function has been defined in global scope, and it is then used as a method of an object, this refers to the object it is contained within.

var width = 600,
var shape = (width:300);

var showWidth = function (){
    document.write(this.width);

}
shape.getWidth = showWidth;
shape.getWidth();

### RECAP: STORING DATA

1. **VARIABLES**
In JavaScript, data is represented using name/value pairs.
To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.

* A variable has just one key (the variable name) and one value.

* Variable names are separated from their value by an equals sign (the assignment operator):

var hotel= 'Quay' ;

2. ARRAYS
* Arrays can store multiple pieces of information.
* Each piece of information is separated by a comma.
The order of the values is important because items in an array are assigned a number (called an index).

* Values in an array are put in square brackets, separated by commas:
var hotels = ['Quay ' ,' Park' , ' Beach' ,'Bloomsbury']

* If you want to access items via a property name or key, use an object (but note that each key in the object must be unique).
If the order of the items is important, use an array.

[Object-access](images/Object-access.jpg)






