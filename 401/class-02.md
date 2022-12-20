# Class 2 Notes - Testing and Modules

[Back to Home](../README.md)

### [In Tests We Trust - TDD in Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

+ Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
+ But Test-Driven Development is a strategy to think (and write!) tests first.
+ A convention widely used is the AAA: Arrange, Act and Assert.
+ Arrange: you need to organize the data needed to execute that piece of code (input);
+ Act: here you will execute the code being tested (exercise the behaviour);
+ Assert: after executing the code, you will check if the result (output) is the same as you were expecting.
+ The cycle:
  + 🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
  + ✅ Write the feature and make the test pass! (you can dance after that)
  + Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)

### [If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

+ Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
+ If you import this script as a module in another script, the __name__ is set to the name of the script/module.
+ Python files can act as either reusable modules, or as standalone programs.
+ if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

### [Recursion](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)

+ The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called a recursive function.
+ Recursion uses more memory, because the recursive function adds to the stack with each recursive call, and keeps the values there until the call is finished. The recursive function uses LIFO (LAST IN FIRST OUT) Structure just like the stack data structure.

### [What on Earth is Recursion - video](https://www.youtube.com/watch?v=Mv9NEXX1VHc)

### [Python Modules and Packages Companion - Video](https://realpython.com/courses/python-modules-packages/)

## Bookmark and Review

### [Google for Education: Python Lists](https://developers.google.com/edu/python/lists)
### [Google for Education: Python Strings](https://developers.google.com/edu/python/strings)
### [Python Modules and Packages](https://realpython.com/python-modules-packages/)
### [Pytest Documentation](https://docs.pytest.org/en/latest/)
### [PyTest Tutorial - up to section "Running test in parallel"](https://www.guru99.com/pytest-tutorial.html)
