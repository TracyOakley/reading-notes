# Class 14 Notes - CSS Transforms and Transitions & Animations

[Back to Home](../README.md)

#### Bookmarks - []

## [CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

1) What does a CSS transform allow the developer to do to an element?

+ With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.
+ Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. 

2) Provide an example of a transform and how you could see that being used on a website.

+ `transform: scale(1.25);` on a mouse over for a button or to get the users attention
+ The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.

## [CSS Transitions and Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

1) What does a CSS transition allow the developer to do to an element?

+ With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
+ As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.
+ There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.
+ In the example below the box will change its background color over the course of 1 second in a linear fashion.
+ `.box {`  
  `background: #2db34a;`  
  `transition-property: background;`  
  `transition-duration: 1s;`  
  `transition-timing-function: linear;`  
}  
`.box:hover {`  
  `background: #ff7b29;`  
}  

2) How does a CSS animation differ from a CSS transition?

+ Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

## [8 Simple CSS3 transitions to WoW!](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)

1) What are some benefits to using CSS transitions on websites?

+ CSS3 has introduced countless possibilities for UX designers, and the best thing about them is that the coolest parts are really simple to implement.
+ Fade in , color change, grow and shrink, rotate, *Swing*, 

2) How this topic fit in with your long-term goals?

+ To have a successful software product, software responsiveness that adhers to the user expectations or responsiveness that assists the user in using the product is fundamental to a good experience and a repeat customer or a referal.
