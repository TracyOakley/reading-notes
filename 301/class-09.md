# Class 9 Notes - Functional Programming

[Back to Home](../README.md)

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. What is functional programming?

+ Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

2. What is a pure function and how do we know if something is a pure function?

+ It returns the same result if given the same arguments (it is also referred as deterministic)
+ It does not cause any observable side effects


3. What are the benefits of a pure function?

+ The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts

4. What is immutability?

+ Unchanging over time or unable to be changed.
+ When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

5. What is Referential transparency?

+ Basically, if a function consistently yields the same result for the same input, it is referentially transparent.
+ pure functions + immutable data = referential transparency

## [Node JS Tutorial for Beginners #6](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?

+ just another javavscript file

2. What does the word ‘require’ do?

+ opens a path using the global object to find and bring in available functionality from the file path

3. How do we bring another module into the file the we are working in?

+ require('filename')

4. What do we have to do to make a module available?

+ module.exports = 'function or code to bring in'
