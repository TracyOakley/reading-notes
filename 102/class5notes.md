# Class 5 Notes - CSS

[Back to Home](../README.md)

[CSS - What it is](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)
[CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)  

[Myers Web Reset Stylesheet](https://meyerweb.com/eric/tools/css/reset/)  

CSS (Cascading Style Sheets) allows you to create great-looking web pages.  

CSS can be used for very basic document text styling — for example, for changing the color and size of headings and links. It can be used to create a layout — for example, turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as animation.  

## CSS Syntax

CSS is a rule-based language — you define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page.

Code Example
h1 {  
    color: red;  
    font-size: 5em;  
}  

1. h1 is the **Selector**
2. Curly brackets
3. one or more declarations, which take the form of **Property** and **Value** pairs.

## [How to Add Css](https://www.w3schools.com/css/css_howto.asp)

Three Ways to Insert CSS
There are three ways of inserting a style sheet:

### External CSS  
External styles are defined within the link element, inside the head section of an HTML page:  

head open tak  
link rel="stylesheet" href="mystyle.css"  
head   

### Internal CSS

Internal styles are defined within the style element, inside the head section of an HTML page

### Inline CSS

Inline styles are defined within the "style" attribute of the relevant element  

h1 style="color:blue;text-align:center;"

## [CSS Color Property](https://www.w3schools.com/cssref/pr_text_color.asp)  

body {
  color: red;
}  

h1 {
  color: #00ff00;
}

p.ex {
  color: rgb(0,0,255);
}  

## Types of Selectors

+ Type is the basic selector
+ Class is the .box example
+ ID Selector #unique { }
+ Attribute Selectors a[title]{}
+ pseudo-classes a:hover{} to style different state of element

## [Box model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

2 types of boxes
+ **Block Boxes**
+ **Inline Boxes**

Boxes have an inner display and an outer display type.

### Outer Display type

if outer diplay is type block then the box will break onto a new line
width and height are respected  
box will extend in the inline direction becoming as wide as its container

if outer display has a type of inline then the box will not break onto a new line


