# Class 8 Notes - CSS Layout Flexbox

[Back to Home](../README.md)

## [CSS Layout](https://web.dev/learn/css/layout/)

## [CSS Flexbox](https://web.dev/learn/css/flexbox/)

1) Flexbox is designed for one-dimensional content. Explain what this means.

+ They can display as a row, or a column.
+ They respect the writing mode of the document.
+ They are single line by default, but can be asked to wrap onto multiple lines.
+ Items in the layout can be visually reordered, away from their order in the DOM.
+ Space can be distributed inside the items, so they become bigger and smaller according to the space available in their parent.
+ Space can be distributed around the items and flex lines in a wrapped layout, using the Box Alignment properties.
+ The items themselves can be aligned on the cross axis.

2) Explain the difference between the main axis and cross axis.

+ The key to understanding flexbox is to understand the concept of a main axis and a cross axis. The main axis is the one set by your flex-direction property. If that is row your main axis is along the row, if it is column your main axis is along the column.

3) How can using certain properties of flexbox negatively impact accessibility?

+ Reversing the flow of items and accessibility
You should be cautious when using any properties that reorder the visual display away from how things are ordered in the HTML document, as it can negatively impact accessibility. The row-reverse and column-reverse values are a good example of this. The reordering only happens for the visual order, not the logical order. This is important to understand as the logical order is the order that a screen reader will read out the content, and anyone navigating using the keyboard will follow.

## [CSS Flexbox - FlexFlow Shorthand](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox#flex-flow_shorthand)

1) What are some advantages of using flexbox over float?

The following simple layout designs are either difficult or impossible to achieve with such tools in any kind of convenient, flexible way:

+ Vertically centering a block of content inside its parent.
+ Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
+ Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.


2) How does this topic connect with your long term goals?

+ Well I think we are finally approaching the methods that modern browers use to create sites and apps, so our sites will finally not feel like from the 1990s.
