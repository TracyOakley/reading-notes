# Class 7 Notes - Object-Oriented Programming, HTML Tables

[Back to Home](../README.md)

## [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

+ Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

Why we need domain modeling?

+ A **domain model** that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. *As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams*.

## [HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

[Advanced HTML Table Features and Accessibility](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced)

1) Why should tables not be used for page layouts?

+ Layout tables reduce accessibility for visually impaired users: screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screen readers' output will be confusing to their users.

+ Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.

+ Tables are not automatically responsive: When you use proper layout containers (such as `<header>, <section>, <article>, or <div>`), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices

2) List and describe 3 different semantic HTML elements used in an HTML `<table>`.

+ `<table>` the content of every table is enclosed by this tag
+ `<tr>` to stop the row from growing use this tag to contain the data
+ `<td>` smallest container inside a table is a table data

## [JavaScript Constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

1) What is a constructor and what are some advantages to using it?

+ A constructor is just a function called using the new keyword.
+ to define the "shape" of an object — the set of methods and the properties it can have — and then create as many objects as we like, just updating the values for the properties that are different.


2) How does the term this differ when used in an object literal versus when used in a constructor?

+ in object literal  you have to use *this* in functions to invoke a property.
+ in a contructor each property has to use the this to set the property and create methods

## [Javascript Prototypes](https://ui.dev/beginners-guide-to-javascript-prototype)

1) Explain prototypes and inheritance via an analogy from your previous work experience.

+ prototypes are usually simple, scaled down versions of larger products to test certain features or behaviors
+ inheritance - money that you get from someone when they die.
