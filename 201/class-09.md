# Forms and JS Events

## HTML Forms

An HTML form is used to collect user input. The user input is most often sent to a server for processing.

The < form> Element

The HTML < form> element is used to create an HTML form for user input:

[Forms](images/forms.png)

[FormWork](images/formwork.png)

### The <input> Element

[FormElement](images/formelement.png)

### Lists, Tables and Forms in CSS

* There are several CSS properties that were created to work with specific types of HTML elements, such as lists, tables, and forms.

### CSS Forms

* The look of an HTML form can be greatly improved with CSS:

[CSS-Forms](images/cssforms.png)

* Whenever you want to collect information from visitors you will need a form, which lives inside a < form> element.

* Information from a form is sent in name/value pairs.

* Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.

* HTML5 introduces new form elements which make it easier for visitors to fill in forms.


### CSS Tables

* The look of an HTML table can be greatly improved with CSS:

[Table-CSS](images/tablescss.jpg)

* Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.

### CSS Lists

List markers can be given different appearances using the list-style-type and list-style image properties.

All CSS List Properties
[Listproperty](images/listproperty.jpg)


* List markers can be given different appearances using the list-style-type and list-style image properties.

* Forms are easier to use if the form controls are vertically aligned using CSS.
* Forms benefit from styles that make them feel more interactive.



***

# JavaScript Events

## HTML events are "things" that happen to HTML elements.

## When JavaScript is used in HTML pages, JavaScript can "react" on these events.

#### Event handlers can be used to handle, and verify, user input, user actions, and browser actions:

* Things that should be done every time a page loads.
* Things that should be done when the page is closed.
* Action that should be performed when a user clicks a button.
* Content that should be verified when a user inputs data.

#### Many different methods can be used to let JavaScript work with events:

* HTML event attributes can execute JavaScript code directly.
* HTML event attributes can call JavaScript functions.
* You can assign your own event handler functions to HTML elements.
* You can prevent events from being sent or being handled.

#### Event Flow

[Event-Flow](images/eventflow.jpg)

* Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).

* Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.

* When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.

* You can use event delegation to monitor for events that happen on all of the children of an element.

* The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events

#### FORM EVENTS

[Form-Event](images/formevent.jpg)

#### MOUSE EVENTS

[MouseEvent](images/mouseevent.png)


