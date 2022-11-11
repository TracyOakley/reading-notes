# Class 5 Notes - Thinking in React

[Back to Home](../README.md)

## [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the single responsibility principle and how does it apply to components?

+ But how do you know what should be its own component? Use the same techniques for deciding if you should create a new function or object. One such technique is **the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.**

2. What does it mean to build a ‘static’ version of your application?

+ Now that you have your component hierarchy, it’s time to implement your app. The easiest way is to build **a version that takes your data model and renders the UI but has no interactivity.** It’s best to decouple these processes because building a static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and not a lot of typing. We’ll see why.
+**To build a static version of your app that renders your data model,** you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

3. Once you have a static application, what do you need to add?

+ Make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with **state.**
+  **The key here is DRY: Don’t Repeat Yourself. Figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand.**

4. What are the three questions you can ask to determine if something is state?

  1. Is it passed in from a parent via props? If so, **it probably isn’t state.**
  2. Does it remain unchanged over time? **If so, it probably isn’t state.**
  3. Can you compute it based on any other state or props in your component? **If so, it isn’t state.**


5. How can you identify where state needs to live?

+ **Remember: React is all about one-way data flow down the component hierarchy. It may not be immediately clear which component should own what state. This is often the most challenging part for newcomers to understand, so follow these steps to figure it out:**

For each piece of state in your application:

+ Identify every component that renders something based on that state.
+ Find a common owner component (a single component above all the components that need the state in the hierarchy).
+ Either the common owner or another component higher up in the hierarchy should own the state.
+ If you can’t find a component where it makes sense to own the state, **create a new component solely for holding the state** and add it somewhere in the hierarchy above the common owner component.


## [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”?

+ Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

+ line 2 returns a function that takes one parameter (m) and the function will compare the one parameter (m) to the argument (n)

3. Explain how either map or reduce operates, with regards to higher-order functions.

+ The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.
+ Another common thing to do with arrays is to compute a single value from them. Our recurring example, summing a collection of numbers, is an instance of this. Another example is finding the script with the most characters.
The higher-order operation that represents this pattern is called reduce (sometimes also called fold). It builds a value by repeatedly taking a single element from the array and combining it with the current value. When summing numbers, you’d start with the number zero and, for each element, add that to the sum.
