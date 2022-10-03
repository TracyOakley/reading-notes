# Class 1 Notes - "Getting Started with Web Development"

[Back to Home](../README.md)

## [Getting started with the Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web) 
This website has alot of good info.

1) My short poem: "HTTP Sends Request"

+ My browser first finds the real address
+ it finds it on the DNS,
+ the browser then sends a request to the server,mmK
+ when the server approves, "200 OK"
+ and starts sending the websites files back .
+ My browser then displays as easy as that.

2) Describe how HTML, CSS, and JS files are “parsed” in the browser.

Answer from [https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

  a) The browser parses the HTML file first, and that leads to the browser recognizing any `<link>` -element references to external CSS stylesheets and any `<script>`-element references to scripts.

  b) As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from `<link> `elements, and any JavaScript files it has found from `<script>` elements, and from those, then parses the CSS and JavaScript.

  c) The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.

  d) As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

3) How can you find images to add to a Website?

+ You own the image.
+ You have received explicit, written permission from the image owner.
+ You have ample proof that the image is, in fact, in the public domain. (Use Google images and tools with creative commons license.)


4) How do you create a String vs a Number in JavaScript?

+ Use String by placing inside "double quotes" or 'single quotes' i.e. let string = "string";
+ Use a number by not using quotes i.e. let number = 7;

5) What is a Variable and why are they important in JavaScript?

+ Variables are containers that store values. 
+ Variables are necessary to do anything interesting in programming. If values couldn't change, then you couldn't do anything dynamic.


## Intro to HTML
(Amswers from this section are from: [https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started))

1) What is an HTML attribute?
+ Attributes contain extra information about the element that won't appear in the content. In this example, the class attribute is an identifying name used to target the element with style information.

2) Describe the Anatomy of an HTML element.
+ Opening tag, content and closing tag.

3) What is the Difference between `<article>` and `<section>` element tags?

+ article - encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).
+ section - it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. 

4) What Elements does a “typical” website include?
+ DOCTYPE, HTML, head, body, Meta, title, header, nav,  main, footer.

5) How does metadata influence Search Engine Optimization?

+ Specifying a description that includes keywords relating to the content of your page is useful as it has the potential to make your page appear higher in relevant searches performed in search engines.
+ Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document.

6) How is the `<meta>` HTML tag used when specifying metadata?

Many <meta> elements include name and content attributes:

+ name specifies the type of meta element it is; what type of information it contains.
+ content specifies the actual meta content.

`<meta name="author" content="Chris Mills" />
<meta
  name="description"
  content="The MDN Web Docs Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing web sites and applications." />`




## Website Design

1) What is the first step to designing a Website?

+ Project ideation from [https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding)

2) What is the most important question to answer when designing a Website?

+ What do you want to accomplish?

## [Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)

1) Why should you use an `<h1>` element over a `<span>` element to display a top level heading?

+ Semantic Element like h1, which gives the text it wraps around the role (or meaning) of "a top level heading on your page, while span can look like a h1 with the correct CSS, it will lack the semantics that the browser interprets.

2) What are the benefits of using semantic tags in our HTML?

+ Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
+ Screen readers can use it as a signpost to help visually impaired users navigate a page
+ Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
+ Suggests to the developer the type of data that will be populated
+ Semantic naming mirrors proper custom element/component naming

## [What is Javascript?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript#what_is_javascript_doing_on_your_page)

1) Describe 2 things that require JavaScript in the Browser?

+ displaying timely content updates
+ animated 2D/3D graphics
+ interactive maps

2) How can you add JavaScript to an HTML document?

+ Internal - add javascript code inside our `<script>` element
+ External - add javascript code in an external file by addind a src attribute to a script element `<script src="script.js"></script>`
+ Inline by adding JS code inside HTML.
