# Class 4 Notes - React and Forms

[Back to Home](../README.md)

## [React Docs - Forms](https://reactjs.org/docs/forms.html)

1. What is a ‘Controlled Component’?

+ In HTML, form elements such as `<input>, <textarea>, and <select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().
+ We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. **An input form element whose value is controlled by React in this way is called a “controlled component”**

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

+ Since the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since `handleChange` runs on every keystroke to update the React state, the displayed value will update as the user types.

3. How do we target what the user is entering if we have an event handler on an input field?

+ It can sometimes be tedious to use controlled components, because you need to write an event handler for every way your data can change and pipe all of the input state through a React component. This can become particularly annoying when you are converting a preexisting codebase to React, or integrating a React application with a non-React library. In these situations, you might want to check out uncontrolled components, an alternative technique for implementing input forms.

## [The Conditional Ternary Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

1. Why would we use a ternary operator?

+ Shorten your **if** statements into one line of code with the conditional *?* operator

2. Rewrite the following statement using a ternary statement:

`if(x===y){`
  `console.log(true);`
`} else {`
  `console.log(false);`
`}`

+ (x===y) ? console.log(true) : console.log(false);

## Bookmark and Review

+ [React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)
+ [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)
