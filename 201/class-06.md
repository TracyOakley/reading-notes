# Class 6 Notes - Problem Domain, Objects and the DOM

[Back to Home](../README.md)

## [Understanding the Problem Domain](https://simpleprogrammer.com/solving-problems-breaking-it-down/)

+ When most programmers are given a programming problem in an interview, they make several key mistakes.  The most severe of those is the improper allocation of time.

+ The most common mistake I see when conducting interviews or watching someone try to solve a programming problem is they try to start writing code as soon as possible.

+ 1) Read the problem completely twice.
+ 2) Solve the problem manually with 3 sets of sample data.
+ 3) Optimize the manual steps.
+ 4) Write the manual steps as comments or pseudo-code.
+ 5) Replace the comments or pseudo-code with real code.
+ 6) Optimize the real code.
+ As much as 70% of our time should be spent in steps 1-3.

## [Difference btw JS Object Ref and Primative Values](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)

+ All data types in JavaScript can be put into one of two categories: primitive values and object references.

+ Primitive values and object references behave differently. This difference in behavior affects how variable assignments are made, how equality operators get their results, and how JavaScript programs run in general. Understanding the difference between primitive values and object references is critical to mastering JavaScript as a programming language. 

+ primitive value is assigned to a variable (eg let foo = ‘bar’), the variable is set to that value directly.

+ When the variable is assigned with an object, however, things are different. Instead of containing the value directly, that variable contains a reference to it.

+ One key difference between primitive values and object references is mutability. Primitive values are immutable and object references are mutable.

+ JavaScript currently supports eight data types. All of these data types (Booleans, Null, Undefined, Number, BigInt, String, Symbol) are primitive values except for object references.

+ data types such as arrays, functions, and dates are object references under the hood.

## [JS Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

1) How would you describe an object to a non-technical friend you grew up with?

+ A collection of related data and/or functionality. These usually consist of several variables and functions (which are called properties and methods when they are inside objects).

2) What are some advantages to creating object literals? 

+ When you want to transfer a series of structured, related data items in some manner, for example sending a request to the server to be put into a database. Sending a single object is much more efficient than sending several items individually

3) How do objects differ from arrays?

+ object is easier to work with than an array, when you want to identify individual items by name

4) Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

+ if an object property name is held in a *variable*, then you can't use dot notation to access the value, but you can access the value using bracket notation

5) Evaluate the code below. What does the term this refer to and what is the advantage to using this?  

const dog = {  
  name: 'Spot',  
  age: 2,  
  color: 'white with black spots',  
  humanAge: function (){  
    console.log(`${this.name} is ${this.age*7} in human years`);  
  }  
}

+ **this** keyword refers to the current object the code is being written inside — so in this case this is equivalent to dog

## [Introduction to the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) this is great information!

1) What is the DOM?

+ (DOM) is the data representation of the objects that comprise the structure and content of a document on the web.

+ Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.

2) Briefly describe the relationship between the DOM and JavaScript.

+ All of the properties, methods, and events available for manipulating and creating web pages are organized into objects. 

+ The DOM is built using multiple APIs that work together. The core DOM defines the entities describing any document and the objects within it. This is expanded upon as needed by other APIs that add new features and capabilities to the DOM

+ That is to say, it is written in JavaScript, but uses the DOM to access the document and its elements. The DOM is not a programming language, but without it, the JavaScript language wouldn't have any model or notion of web pages, HTML documents, SVG documents, and their component parts. 

+ The DOM is not part of the JavaScript language, but is instead a Web API used to build websites. JavaScript can also be used in other contexts. For example, Node.js runs JavaScript programs on a computer, but provides a different set of APIs, and the DOM API is not a core part of the Node.js runtime.
