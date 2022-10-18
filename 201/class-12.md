# Class 12 Notes - JS Canvas and Chart.js

[Back to Home](../README.md)

#### [Canvas - Drawing Shapes](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes) and [Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors) and [Drawing Text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

## [Javascript Canvas](https://www.javascripttutorial.net/web-apis/javascript-canvas/)

1) What does the `<canvas>` allow a developer to acheive?

+ element that allows you to draw 2D graphics using JavaScript

2) What is the importance of the closing `</canvas>` tag?

+ element requires the closing tag `</canvas>`. Any content between the opening and closing tags is fallback content that will display only if the browser doesn’t support the `<canvas>` element.

3) Explain what the getContext() method does.

+ features the getContext() method that returns a render context object.
+ The getContext() takes one argument which is the type of context. For example, you use the "2d" to get a 2D rendering context object, which is an instance of the CanvasRenderingContext2D interface.
+ The 2D rendering context allows you to draw shapes, text, images, and other objects
+ Use the fillStyle and StrokeStyle properties to set the styles for the 2D drawing context.

## [Chart.js Documentation](https://www.chartjs.org/docs/latest/)

1) What is Chart.js and how it can be brought into your project?

+ Chart.js is how you can draw charts
+ Bring into project with canvas tag and `<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>`

2) List 3 different Chart types you can create using Chart.js.

+ Area, Bubble, line and Bar. 

## [Animated Charts with charts.js](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

1) What are some advantages to displaying data via a chart over a table?

+ Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

2) How could Chart.js aid your previously created applications visually?

+ We could add a bar graph or a pie graph to the Salmon Cookies to improve the readability of the data.
