<h1>Java Script</h1>

Java Script is a scripting or programming language that allows you to implement complex faetures on web pages

It brings interactivity to the web pages.

<h2>1. Variables</h2>

Variables are the containers for storing data values.

var, const and let are the reserved keywords to declare a variable.

JavaScript identifiers are case-sensitve.

You can assign a value to a variable using equal to (=) operator when you declare it or before using it.

![alt text](image-1.png)

const and let also support global scope but unlike var they does not create a property on global object.

    e.g:
    var x = "global"
    let y = "global";
    console.log(this.x); // "global"
    console.log(this.y); // undefined

let variables can be updated but not re-declared.

const variables can neither be updated not re-declared.

<h2> 2. Data types in JS </h2>
    There are 8 basic data types in JavaScript
    <ul>
    <li>number</li>
    <li>string</li>
    <li>boolean</li>
    <li>bigInt // if the number is appended with n at end its bigInt</li>
    <li>undefined</li>
    <li>null // when we check the type we will get object but its mistake in JS and fixing it would break the internet</li>
    <li>object</li>
    <li>Symbol // var sym = Symbol("id")</li>
    </ul>
    Rest all types are Objects in some form.

<h2>3. Null vs Undefined</h2>

![alt text](image-2.png)

Equality Comparison
<li>== This operator does value comparison.</li>
<li>=== This operator does value plus data type comparsion.</li>

<h2>4. Spread Operator</h2>

The operator's shape is three consecutive dots and is written as: ...

<b>Usages of spread operator : </b>

<li><b>Expanding String</b> -  Convert string into list of array </li>
<li><b>Combining Arrays</b> - Combine array or add value to array</li>
<li><b>Combining Object</b> - Combine Object or add value to object</li>
<li>Creating New Shallow Copy of Arrays and objects </li>
<h2>5. Destructuring</h2>

The two most used data structures in JavaScript are Object and Array.

Destructuring is a special syntax that allows us to "unpack" arrays or objects into a bunch of variables, as sometimes that's more convenient.

<li>Array destructuring</li>
<li>Object destructuring</li>

<h2>6. String Interpolation</h2>

String interpolatoin allows you to embed expressions in the string.

Template string use back-ticks(``) rather than the singel or double-quotes.

<h2>7. String Methods</h2>

Java Script provides Many metodes to play with strigns. Below are the some of the most commonly used strings method in LWC.

<ol>
    <li>includes()</li>
    <li>indexOf()</li>
    <li>startsWith()</li>
    <li>slice()</li>
    <li>toLowerCase()</li>
    <li>toUpperCase()</li>
    <li>trim()</li>
</ol>

<h2>8. Object/ JSON Operations</h2>
<ol>
    <li>Object.keys()</li>
    <li>Object.values()</li>
    <li>JSON.stringify()</li>
    <li>JSON.parse()</li>
</ol>

<h2>9. Array Methods</h2>
<ol>
    <li><b>map()</b> - loop over the array and return new array based on the value return.</li>
    <li><b>every()</b> - return true or false if every element in the array satisfy the condition.</li>
    <li><b>filter()</b> - return new array with all the elemnts that satisfy the condition</li>
    <li><b>some()</b> - return true if at least one element in the array satisfy.</li>
    <li><b>sort()</b> - sort the elements of an array</li>
    <li><b>reduce()</b> - This method reduces the array to a singel value (left to right)</li>
    <li><b>forEach()</b> - This method calls for each array element.</li>
</ol>

<h2>10. Promise</h2>

Promise is an object that may produce a single value sometime in the future.

Promise are used to handle asynchronous operations in JavaScript.

<b>A promise has 3 states:</b>
    ![alt text](image-3.png)
<ol>
<li>pending()</li>
<li>fulfilled()</li>
<li>rejected()</li>
</ol>

Use case from LWC point of view
<ul>
    <li>Ferching data from server</li>
    <li>Loading file from system</li>
</ul>

<h2>11. Modules Import & Export</h2>

<h3>Exports: </h3>

<b>Exporting</b> - Use export keyword to export many variable or many method from a file

    e.g 1: export const name = 'vineeth'

    e.g 2: export function getName(){
    return 'vineeth'
    }

<b>Default export</b> - Use export default keyword to export only one variable or a method from a file

    e.g: export default user = 'salesforce'

<h3>Imports:</h3>

<b>Importing</b> - use import keyword to import variable or method from a given file path or module.

    Multiple imports : `import {name, getName} from "./filepath"`

    Imports all exported members : import * as Utils from "./filepath"

    Imports a module with a default member: import user from "./filepath"

<h2>12. Query Selector</h2>

<b>querySelector</b> - The querySelector() method returns the first element that matches a specified CSS selector(s) in the docment.

    e.g: document.queySelector(selector);

<b>querySelectorAll</b> - The querySelectorAll() method returns all element in the docuent that matches a specified CSS selector(s) as a static NodeList object.

    e.g: document.querySelectorAll(selector);

<h2>13. Event</h2>

An event is an action that occurs in the web browser, which the web browser feedbacks to you so that you can respond to it.

For example, when users click a button on a webpage, you may want to respond to this click event by displaying a alert box.

<b>Event handler</b> - It is a block of code that will execute when the event occurs. It is also known as an event listener.

Two common ways to add events:

1. <b>HTML Event Handler attribute</b> - When we add event through HTML, Event always begin with on keyword like onclick, onchange, onkeyup.

2. <b>Event Listener</b> - Event Handlers provide two main methods for dealing with the registering/deregistering event listeners:
    <ul>
    <li><b>addEventListener() </b>- register an event handler</li>
    <li><b>removeEventListener() </b>- remove an event handler</li>
    </ul>

    <b>Event Propagation</b> - event propagtion explains the order in which events are recived on the page from the element where the event occurs and propagated through the DOM tree.

    There are two main event models:
    1. <b>Event Bubbling</b> - In the event bubbling model, an event starts at the most specific element and then flows upward toward the least specific element (the document or even window)
    ![alt text](image-4.png)

    2. <b>Event Capturing</b>
    Custom Event
    In Java Script we can create our own custom event using Custom Event constructor
    syntax: new customEvent("eventName",{options})
    e.g : ![alt text](image-5.png)

<h2>14. Arrow Function</h2>
Arrow functions allow us to write shorter function syntax

![alt text](image-6.png)

Benefits of Arrow functions:
<li>Arrow syntax automatically binds this to the surrounding code's contex</li>

<h2>15. setTimeout vs setInterval</h2>

<b>setTimeout</b> - The setTimeout() is a method of the window object. The setTimeout() sets a timer and executes a callback function after the timer expires.

<b>setInterval</b> - The setInterval() is a method of the window object. The setInterval() repeatedly calls a function with a dealy between each call.
