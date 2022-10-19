# Class 13 Notes - Local Storage and its Future in Web Apps

[Back to Home](../README.md)

### [DiveintoHTML5-Storage](https://github.com/html5doctor/diveintohtml5/blob/gh-pages/storage.html)

## [Local Storage and how to use it On Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

1) Why would a developer use local storage for a web application?

+ The main problem with HTTP as the main transport layer of the Web is that it is stateless. This means that when you use an application and then close it, its state will be reset the next time you open it.

2) What information should not be stored in local storage?

+ Sensitive, private, personal-identifiying information Or Financial info

3) Local storage can store what type of data? How would you convert it to that type before storing?

+ strings, json.stringify

## General Info

+ `localStorage.setItem('favoriteflavor','vanilla');`
+ `var taste = localStorage.getItem('favoriteflavor');`
// -> "vanilla"
+ `localStorage.removeItem('favoriteflavor');`
+  You can also use sessionStorage instead of localStorage 
+ One annoying shortcoming of local storage is that you can only store strings in the different keys. This means that when you have an object, it will not be stored the right way.
+ You can work around this by using the native JSON.stringify() and JSON.parse() methods:
+ `localStorage.setItem( 'car', JSON.stringify(car) );`
+ `console.log( JSON.parse( localStorage.getItem( 'car' ) ) );`

*And the link has examples of how to use it to maintain the state of an interface.*
