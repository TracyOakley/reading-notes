# Class 9 Notes - HTML Forms and JS Events

[Back to Home](../README.md)

## [HTML Input Types](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)

## [Event Reference and listings](https://developer.mozilla.org/en-US/docs/Web/Events)

## [HTML Web forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

1) Why are forms so important in web development?

+ Web forms are a very powerful tool for interacting with users — most commonly they are used for collecting data from users, or allowing them to control a user interface.
+ Web forms are one of the main points of interaction between a user and a website or application. Forms allow users to enter data, which is generally sent to a web server for processing and storage (see Sending form data later in the module), or used on the client-side to immediately update the interface in some way (for example, add another item to a list, or show or hide a UI feature).

2) When designing a form, what are some key things to keep in mind when it comes to user experience?

+ From a user experience (UX) point of view, it's important to remember that the bigger your form, the more you risk frustrating people and losing users. Keep it simple and stay focused: ask only for the data you absolutely need.
+ 

3) List 5 form elements and explain their importance.

1) *form* - This element formally defines a form. It's a container element like a `<section>` or `<footer>` element, but specifically for containing forms; it also supports some specific attributes to configure the way the form behaves. All of its attributes are optional, but it's standard practice to always set at least the action and method attributes:

+ The action attribute defines the location (URL) where the form's collected data should be sent when it is submitted.
+ The method attribute defines which HTTP method to send the data with (usually get or post).

2) *label* - input field for the name is a single-line text field.
3) *input* - input field for the e-mail is an input of type email: a single-line text field that accepts only e-mail addresses
4) *textarea* - a multiline text field
5) *button* - element also accepts a type attribute — this accepts one of three values: submit, reset, or button.

A click on a submit button (the default value) sends the form's data to the web page defined by the action attribute of the <form> element.
A click on a reset button resets all the form widgets to their default value immediately. From a UX point of view, this is considered bad practice, so you should avoid using this type of button unless you really have a good reason to include one.
A click on a button button does nothing! That sounds silly, but it's amazingly useful for building custom buttons — you can define their chosen functionality with JavaScript.

## [JS Intro to Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

1) How would you describe events to a non-technical friend?

+ Events are actions or occurrences that happen in the system you are programming, which the system tells you about so your code can react to them.

2) When using the addEventListener() method, what 2 arguments will you need to provide?

+  the name of the event and a function to handle the event.

3) Describe the event object. Why is the target within the event object useful?

+ Sometimes, inside an event handler function, you'll see a parameter specified with a name such as event, evt, or e. This is called the event object, and it is automatically passed to event handlers to provide extra features and information.

4) What is the difference between event bubbling and event capturing?

+ the event bubbles up from the innermost element that was clicked.
+ This behavior can be useful and can also cause unexpected problems. 
+ Captureing -browser checks to see if the element's outer-most ancestor (`<html>`) has a click event handler registered on it for the capturing phase, and runs it if so.
Then it moves on to the next element inside `<html>` and does the same thing, then the next one, and so on until it reaches the direct parent of the element that was actually clicked
