# Class 3 Notes - Passing Functions as Props

[Back to Home](../README.md)

## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

1. What does .map() return?

+ Returns a new array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

+ `const numbers = [1, 2, 3, 4, 5];
+ const listItems = numbers.map((number) =>
+ `<li>`{number}`</li>`
);`

3. Each list item needs a unique ____.

+ **Key**

4. What is the purpose of a key?

+ Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

+ const listItems = numbers.map((number) =>
  `<li` key={number.toString()}>{number}
  `</li>` );

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

1. What is the spread operator?

+ The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and **spreading an array out into a function’s arguments**.
+ ...

2. List 4 things that the spread operator can do.

+ Math.max([1,2,3]) = Nan but Math.max(...[1,2,3])
+ spread syntax “spreads” the array into separate arguments
+ copying an array
+ adding to state in React
+ Combining objects

3. Give an example of using the spread operator to combine two arrays.

+ const myArray = [1,2,3]
+ const yourArray = [4,5,6]
+ const ourArray = [...myArray,...yourArray]

4. Give an example of using the spread operator to add a new item to an array.

+ const addArray = [...myArray, 3] // add 3 to the array
+ const fewFruit = ['🍏','🍊','🍌']
+ const fewMoreFruit = ['🍉', '🍍', ...fewFruit]

5. Give an example of using the spread operator to combine two objects into one.

+ const objectOne = {hello: "🤪"}
+ const objectTwo = {world: "🐻"}
+ const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}

## [How to Pass functions btw Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

1. In the video, what is the first step that the developer does to pass functions between components?

+ create a function in the parent component where the state you want to change is
+ pass the function to the child through the props in the render()

2. In your own words, what does the increment function do?

+ takes a name parameter and creates an new array using map to increment the state if the name passed in matches

3. How can you pass a method from a parent component into a child component?

+ pass the function to the child through the props in the render()

4. How does the child component invoke a method that was passed to it from a parent component?

+ child just calls it like this.props.increment(this.props.name)


## BookMark and Review

+ [React Tutorial through 'Declaring a Winner'](https://reactjs.org/tutorial/tutorial.html)
+ [React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)
