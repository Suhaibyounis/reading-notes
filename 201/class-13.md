# Local Storage

[Local-Storage](images/localstorage.jpg)


### * Why Store Data on the Client?

    1. The main reason is practicality. JavaScript code running on the browser does not necessarily need to send all information to the server. There are several use cases:

    2. You want to increase performance. You can cache data client-side so it can be retrieved without additional server requests.

    3. You have a significant quantity of client-side-only data, e.g. HTML strings or widget configuration settings.

    4. You want you make your application work off-line.

### JavaScript Variables (Past, Present and Future).

* The simplest choice is JavaScript variables. It may be practical to create a single global variable to store application data


### What is HTML Web Storage?

* With web storage, web applications can store data locally within the user's browser.

* Before HTML5, application data had to be stored in cookies, included in every server request. Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance.

* Unlike cookies, the storage limit is far larger (at least 5MB) and information is never transferred to the server.

* Web storage is per origin (per domain and protocol). All pages, from one origin, can store and access the same data.

### HTML Web Storage Objects

* HTML web storage provides two objects for storing data on the client:

    * window.localStorage - stores data with no expiration date
    * window.sessionStorage - stores data for one session (data is lost when the browser tab is closed)

### The localStorage Object

[Local-Storage](images/localstorage.png)

#### Example explained:

* Create a localStorage name/value pair with name="lastname" and value="Smith"
* Retrieve the value of "lastname" and insert it into the element with id="result"


### STORAGEEVENT OBJECT

[Storage-Event](images/storageevent.png)

Limitations in current browsers:

    * 5 MB of storage from each origin.
    * Can not ask user for more storage (except for Opera, sort of)


### HTML5 in action

[HTML-in-Action](images/htmlInAction.jpg)

[Inaction](images/inaction.jpg)


* In the saveGameState() function, we did not worry about the data type:
    * localStorage[" halma.game.in.progress"] = gGameInProgress;

* But in the resumeGame() function, we need to treat the value we got from   the local storage area as a string and manually construct the proper Boolean value ourselves:
    * gGameInProgress = (localStorage[" halma.game.in.progress"] == "true");

* Similarly, the number of moves is stored in gMoveCount as an integer. In the saveGameState() function, we just stored it:
    * gMoveCount = parseInt(localStorage[" halma.movecount"]);

* But in the resumeGame() function, we need to coerce the value to an integer, using the parseInt() function built into JavaScript:
    * gMoveCount = parseInt(localStorage[" halma.movecount"]);


### Beyond Key/Value Pairs: Competing Visions

[Beyond](images/beyond.jpg)

### Web SQL Database

* The Web SQL Database specification has been implemented by four browsers and platforms

[Beyond-Key](images/beyondkey.png)


















