# HTML Text, CSS Introduction, and Basic JavaScript Instructions.

## **HTML**

## **Text**

* When creating a web page, you add tags known as ***markup*** to the contents of the page.
These tags provide:
1. Extra meaning,
2. Allow browsers to show users the appropriate structure for the page.

* **Type of Markup**:
### 1. **Structural markup** : the elements that use to describe both **Headings** and **Paragraphs**.

### 2. **Semantic markup**:  provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms.

[Books](https://images.adsttc.com/media/images/5b92/c731/f197/cc72/ee00/00c5/large_jpg/IsometricBookCity_5.jpg?1536345898)

* Headings:
There is Six Levels of **Heading Tags** ( from **h1**  for the main Head, then **h2** for the second level of head, ans so on up to **h6**).

* Paragraphs **< p> </ p>**
A paragraph consists of one or more sentences that form a self-contained unit of discourse. The start of a paragraph is indicated by a new line.

* Bold  < b> & Italic < i>
1. By enclosing words in the tags < b > and </ b> we can make characters appear <bold>. 
The <b> element also represents a section of text that would be presented in a visually different way.

2. By enclosing words in the tags < i> and </ i> we can make characters appear italic.
The < i> element also represents a section of text that would be said in a different way from surrounding content.

* Superscript < sup> & Subscript < sub>
The < sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 2<sup>2</sup>.

The < sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H<sub>2</sub>O.

* White Space
In order to make code easier to read, web page authors often add extra spaces or start some elements on new lines.

* Line Breaks & Horizontal Rules
To add a line break inside the middle of a paragraph you can use the line break tag < br/>.

To add a horizontal rule between sections using the < hr/> tag.

***

## Visual Editors & Their Code views

**Visual editors** often resemble word processors. Although each editor will differ slightly, there are some features that are common to most editors that allow you to control the presentation of text.

**Code views** show you the code created by the visual editor so you can manually edit it, or so you can just enter new cod yourself. It is often activated using a button with an icon that says HTML or has angled brackets. White space may be added to the code by the editor to make the code easier to read.

## Semantic Markup
Text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages.

## Strong & Emphasis
The use of the <strong> element indicates that its content has strong importance.

The <em> element indicates emphasis that subtly changes the meaning of a sentence.

## Quotations
There are two elements commonly used for marking up quotations:
1. The < blockquote> element is used for longer quotes that take up an entire paragraph.
2. The < q> element is used for shorter quotes that sit within a paragraph.

## Abbreviations & Acronyms
If you use an abbreviation or an acronym, then the < abbr> element can be used. A title attribute on the opening tag is used to specify the full term.

## Citations & Definitions
1. When you are referencing a piece of work such as a book, film or research paper, the < cite> element can be used to indicate where the citation is from.
2. The < dfn> element is used to indicate the defining instance of a new term.

## Author Details
The <address> element has quite a specific use: to contain contact details for the author of the page.

## Changes to Content
The < ins> element can be used to show content that has been inserted into a document, while the < del> element can show text that has been deleted from it.

The < s> element indicates something that is no longer accurate or relevant (but that should not be deleted).

[Example](201/images/html.jpg)

***

## Introducing CSS

* To understand how **CSS** works is to imagine that there is an invisible box around every **HTML** element.

* **CSS** allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

[CSS-Example](201/images/css-example.jpg)

* CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: **Selector** and **Declaration**. 

* Selectors indicate which element the rule applies to.
* Declarations indicate how the elements referred to in the selector should be styled.

[Selector](201/images/selector.jpg)

* CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.

![Properties](201/images/properties.jpg)

## Using External CSS
* < link>:  The < link> element can be used in an HTML document to tell  he browser where to find the CSS file used to style the page.
* < href> :  This specifies the path to the CSS file.
* < type>: This attribute specifies the type of document being linked to.
* < rel> : This specifies the relationship between the HTML page and the file it is linked to.

[External-CSS](201/images/external-css.jpg)

## Using Internal CSS
< style> You can also include CSS rules within an HTML page by placing them inside a < style> element, which usually sits inside the < head> element of the page.

## When building a site with more than one page, you should use an external CSS style sheet. This:
* Allows all pages to use the same style rules (rather than repeating them in each page).
* Keeps the content separate from how the page looks.
* Means you can change the styles used across all pages by altering just one file (rather than each individual page)

[Internal-CSS](201/images/internal-css.jpg)

## CSS Selectors

[CSS-Selector](201/images/css-selector.jpg)

***

## Why use External Style Sheets?
1. All of your web pages can share the same style sheet. This is achieved by using the **< link>** element on each **HTML** page of your site to link to the same CSS document.

2. If you want to make a change to how your site appears, you only need to edit the one CSS file and all of your pages will be updated.

3. The **HTML** code will be easier to read and edit because it does not have lots of **CSS** rules in the same document.

* If you are just creating a single page, you might decide to put the rules in the same file to keep everything in one place.

* CSS rules usually appear in a separate document, although they may appear within an HTML page. 

*** 
***
***

# Javascript Instructions

* STATEMENTS: A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a **Statement**.
* Statements should end with a semicolon.

* JAVASCRIPT IS CASE SENSITIVE
JavaScript is case sensitive so **hourNow** means something different to **HourNow** or **HOURNOW**.

## STATEMENTS ARE INSTRUCTIONS AND EACH ONE STARTS ON A NEW LINE
* A statement is an individual instruction that the computer should follow. Each one should start on a new line and end with a semicolon. This makes your code easier to read and follow.

* The semicolon also tells the JavaScript interpreter when a step is over, indicating that it should move to the next step.
But,
Some statements are surrounded by curly braces; these are known as code blocks. The closing curly brace is not followed by a semicolon.

## COMMENTS
* You should write comments to explain what your code does.
* They help make your code easier to read and understand.

[Comments](201/images/comments.jpg)

### Types of Comments: 
* Multi-Line Comments
    * used for descriptions of how the script works, or to prevent a section of the script from running when testing it.
    * starting with the / * characters and ending with the * / characters
    * Anything between these characters is not processed by the JavaScript interpreter.

* Single-Line Comments
    * used for short descriptions of what the code is doing.
    * Good use of comments will help you if you come back to your code after several days or months.
    * anything that follows the two forward slash characters I/ on that line will not be processed by the JavaScript interpreter.

## WHAT IS A VARIABLE?
* A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

* A variable is a good name; because the data stored in a variable can change (or vary) each time a script runs.

* variables can be used to represent values in your scripts that are likely to change. The result is said to be **calculated** or **computed** using the data stored in the variables.

### Declaring Variables
* When you create the Variable, you should give it a special **Name**.

[variable](201/images/variable.jpg)

* Assign Value to Variable.

Quantity = 3;
(Quantity --> Variable Name)  (= --> assign operator) (3 --> variable value)

### Data Type:
1. NUMERIC DATA TYPE
    * used for things like calculators
    * used for tasks such as determining the size of the screen, ...

2. STRING DATA TYPE
    * consists of letters and other characters.
    * Note how the string data type is enclosed within a pair of quotes( ' '  // " " )
    * used to add new content into a page and they can contain HTML markup.

3. BOOLEAN DATA TYPE
    * can have one of two va lues: true or false.
    * helpful when determining which part of a script should run.

## USING A VARIABLE TO STORE :
1. A NUMBER

[Assign-Variable-number](201/images/assign-variable.jpg)

2. A STRING

[Assign-Variable-string](201/images/assign-variable-string.jpg)

* Quotes inside **String**
    * If you just want to use double quotes in the string, you could surround the entire string in single quotes, and the same for single quotes.

    * Escaping
Escaping the quotation characters. This is done by using a backwards slash (or "backslash") before any type of quote mark that appears within a string.

3. A BOOLEAN

[BOOLEAN](201/images/boolean.jpg)

## Declaring Variable:

1. Variables are declared and values assigned in the same statement.

2. more than one variable are declared on the same line, then values assigned to each.

3. Two variables are declared and assigned values on the same line.Then one is declared and assigned a value on the next line.

4. variable is used to hold a reference to an element in the HTML page. This allows you to work directly with the element stored in that variable.

[VARIABLE-DECLARING](201/images/variable-declaring.jpg)

### RULES FOR NAMING VARIABLES

1. The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number.
2. The name can contain letters, numbers, dollar sign ($), or an underscore (_).
3. You cannot use keywords or reserved words.
4. All variables are case sensitive.
5. Use a name that describes the kind of information that the variable stores.
6. If the variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.

## ARRAYS
* An array is a special type of variable. It doesn't just store one value; it stores a list of values.

* Arrays are especially helpful when you do not know how many items a list will contain because, when you create the array, you do not need to specify how many values it will hold.

* You create an array and give it a name (using the var keyword followed by the name of the array).

* The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array, and its called **Array literal** .

* **Array constructor** : uses the new keyword followed by Array(); The va lues are then specified in parentheses (not square brackets), and each value is separated by a comma.

## EXPRESSIONS
* An expression evaluates into (results in) a single value.

* Types of expressions?
1. EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE.

[Expression1](201/images/expression1.jpg)

2. EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE.

[Expression2](201/images/expression2.jpg)

## OPERATORS
* Expressions rely on things called operators; they allow programmers to create a single value from one or more values.

Type of Operators:
1. ASSIGNMENT OPERATORS
    * color = 'beige';
2. ARITHMETIC OPERATORS
    * area = 3 * 2;
3. STRING OPERATORS
    * greeting= 'Hi 1 + 'Mol ly';
4. COMPARISON OPERATORS
    * buy = 3 > 5;
5. LOGICAL OPERATORS
    * buy= (5 > 3) && (2 < 4);


*  ARITHMETIC OPERATORS

[Arithmetic-Operators](201/images/arithmetic-operators.jpg)

* STRING OPERATOR
* There is just one string operator: the+ symbol.
* It is used to join the strings on either side of it.

**Concatenation** : the process of joining together two or more strings to create one new string.

[String-Operator](201/images/string-operators.jpg)


[Javascript-Example](201/images/javascript-example.jpg)

***
***
***

# Decisions and Loops

[Decisions-&-Loops](201/images/loops.jpg)

## Components to a decisions: 

1. Evaluation of a Condition.
2. Conditional Statements.

[Condition](201/images/condition.jpg)

## Comparison Operators
1. Equal to " == "
    Operator compares two values ( numbers, strings,Booleans) to see if they are the same.
2. Not equal to "!="
    Operator compares two values ( numbers, strings,Booleans) to see if they are not the same.
3. Strict Equal to "==="
    Operator compares two check that both the data type and values are the same.
4. Strict not Equal to "!=="
    Operator compares two check that both the data type and values are not the same.
5. Greater than ">"
    Operator checks if the numbers on the lift is greater than the numbers on the right.
6. Less than "<"
    Operator checks if the numbers on the lift is less than the numbers on the right.
7. Greater than or equal ">="
    Operator checks if the numbers on the lift is greater than or equal to the numbers on the right.
8. Less than or equal to "<="
    Operator checks if the numbers on the lift is less than or equal to the numbers on the right.

    ***

## Logical Operators
* Comparison operators return single values of true or false.

* Logical and "&&"
    The Operator tests more than one condition.
* Logical Or "||"
    The Operator tests at least one condition.
* Logical not "!"
    The Operator takes a single Boolean value and inverts it.


## Loops
Loops check a condition. If it returns true, a code block will run, and so on will repeat until the condition returns fslse.
* Types of Loops:
1. For, used to run code a specific numbers of times.

2. While, if you don't know how many times the code should run.

* Do While, similar to the while loops, but it will always run the statements inside the curly braces at least once, even the condition evalutes to fslse.

### Loops Counters
* For Loop uses a counter as a condution, and this tell the code to run a specified numbers of times.

* Statements of For Loop:

1. Initialization var i= 0;
2. Condition i < 9;
3. Update i++
* While Loop will continue to run for as long as the condition in parentheses is true.