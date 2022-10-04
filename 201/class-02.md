# Class 2 Notes - Basics of HTML, CSS and JS 

[Back to Home](../README.md)

## HTML

[HTML Text Fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

[HTML Advanced Text Formatting](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)

1) Why is it important to use semantic elements in our HTML?

+ Users looking at a web page tend to scan quickly to find relevant content, often just reading the headings, to begin with. 
+ Search engines indexing your page consider the contents of headings as important keywords for influencing the page's search rankings. Without headings, your page will perform poorly in terms of SEO (Search Engine Optimization).
+ Severely visually impaired people often don't read web pages; they listen to them instead. This is done with software called a screen reader. This software provides ways to get fast access to given text content.
+ To style content with CSS, or make it do interesting things with JavaScript, you need to have elements wrapping the relevant content, so CSS/JavaScript can effectively target it.

2) How many levels of headings are there in HTML?
 + 6

3) What are some uses for the `<sup>` and `<sub>` elements?
 + sup can be used to make 25th or x^2
 + sub can be used to make H20.

4) When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?

+  This is used to wrap around an abbreviation or acronym. When including either, provide a full expansion of the term in plain text on first use, along with the <abbr> to mark up the abbreviation.

## CSS

[How Css is Structured](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)

1) What are ways we can apply CSS to our HTML? 

+ External Stylesheet
+ Internal Stylesheet
+ Inline Styles

2) Why should we avoid using inline styles?

+ It is the opposite of a best practice. First, it is the least efficient implementation of CSS for maintenance. One styling change might require multiple edits within a single web page. Second, inline CSS also mixes (CSS) presentational code with HTML and content, making everything more difficult to read and understand. Separating code and content makes maintenance easier for all who work on the website.

3) Selector h2  
    Declarations color and padding  
    properties black and 5px

## JS

[Javascript Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

1) What data type is a sequence of text enclosed in single quote marks? 
+ String
 2) List 4 types of JavaScript operators.
 + Assignment
 + Comparison (Boolean)
 + Logical
 + Arithmetic
3) Describe a real world Problem you could solve with a Function.
+ Verify Data entered is the correct type of data

[https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)

1) An if statement checks a **condition** and if it evaluates to **true**, then the code block will execute.

2) What is the use of an else if? Lets you test another condition if the prior condition is not true.

3) List 3 different types of comparison operators.
+ ===
+ !=
+ <=

What is the difference between the logical operator && and ||?

+ && AND; allows you to chain together two or more expressions so that all of them have to individually evaluate to true for the whole expression to return true.
+ || OR; allows you to chain together two or more expressions so that one or more of them have to individually evaluate to true for the whole expression to return true.

## [How to write a Git Commit Message](https://chris.beams.io/posts/git-commit/)
