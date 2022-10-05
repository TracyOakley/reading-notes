# Class 3 Notes - HTML Lists, JS Control Flow and CSS Box Model

[Back to Home](../README.md)

## HTML - Ordered and Unordered Lists

[Unordered List Link](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)

1) When should you use an unordered list in your HTML document?

+ For grouping a collection of items that do not have a numerical ordering, and their order in the list is meaningless.  Typically, unordered-list items are displayed with a bullet, which can be of several forms, like a dot, a circle, or a square.  

 2) How do you change the bullet style of unordered list items? 

 + The bullet style is not defined in the HTML description of the page, but in its associated CSS, using the list-style-type property.

 3) When should you use an ordered list vs an unorder list in your HTML document?

+ When the order is meaningful. For example:
+ Steps in a recipe
+ Turn-by-turn directions

4) Describe two ways you can change the numbers on list items provided by an ordered list?

+ `<ol type ="i">`
+ `<ol start="4">`

## CSS - [Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

1) Describe the CSS properties of "margin" and "padding" as characters in a story. What is their role in a story titled: “The Box Model”?

+ Margin is a bouncer and keeps other elements away from the border of the box
+ Padding keeps the border and the content area separate

2) List and describe the four parts of an HTML elements box as referred to by the box model.

+ Content box: The area where your content is displayed; size it using properties like inline-size and block-size or width and height.
+ Padding box: The padding sits around the content as white space; size it using padding and related properties.
+ Border box: The border box wraps the content and any padding; size it using border and related properties.
+ Margin box: The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using margin and related properties.

## JS - [Arrays and Control Flow](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays)

1) What data types can you store inside of an Array?

+ In an array we can store various data types — strings, numbers, objects, and even other arrays. We can also mix data types in a single array — we do not have to limit ourselves to storing only numbers in one array, and in another only strings.

2) Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

+ `const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];`
+ It is a valid array.

3) List five shorthand operators for assignment in javascript and describe what they do.

+ = (assignment), += (addition assignment), %= (remainder assignment), *= (exponential assignment), &&= (logical AND "truthiness")

4) Read the code below and evaluate the last expression and explain what the result would be and why.

+ let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

 + evaluates to `10dog` because false equates to a 0 and 10 + 0 equals 10 and then 10 + dog concatenates to 10dog

 5) Describe a real world example of when a conditional statement should be used in a JavaScript program.

 + when you have to make a decision based on information like based on the time of day should the screen display in dark or light mode or if based on an input compute something.

 6) Give an example of when a Loop is useful in JavaScript.

 + Repeating the same thing over again like asking for the valid input or repeating a task multiple times like performing the way function on every object in an array.
