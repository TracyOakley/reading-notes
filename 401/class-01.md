# Class 1 Notes - Intro to Big O Notation and Python

[Back to Home](../README.md)

## [Pain vs Suffering](https://codefellows.github.io/code-401-python-guide/curriculum/class-01/notes/pain_suffering)

+ Pain is Suffering with a Purpose (but written more eloquently)

## [Intro to Big O Notation](https://robbell.io/2009/06/a-beginners-guide-to-big-o-notation) 

+ Basic intro to 'Constant time' O(1), linear growth O(n), exponential and logarithmic O(log n). Fairly simple and clear.

### [Additional Resources - Audio](https://www.codenewbie.org/basecs/8)

+ Linked List (singlely (point to next neighbor only) and doubly (linked to next and prior neighbor) linked lists)
+ Circular Linked links ( no node that points to null but points to beginning, still has a head node)
+ Big O is how efficient(how fast) algorithm AND data structure perform.
+ insert to front of array O(n)
+ array is good for search and linked links for adding to top
+ Stacks can implement with linked Lists (i.e. call stack)


## [Names and Values in Python - Video](https://www.youtube.com/watch?v=_AEJHKGk9ns) this is really solid presentation and info

+ names, values, assignment and mutability = simple mechanisms
+ names refer to values (through assignment)
+ **Names are reassigned independently**
+ Values live until no references
+ Assignment never copies data! (like array in JS, I think bc mutability)
+ Ints, floats, strings, tuples are immutable types in Python
+ change is unclear, changing Int is 'rebinding', changing array is 'mutating'
+ array .append (mutates) VS = newArray + ... (needs return)
+ Dymanically typed - names (left side of =) have no type and values have no scope (right side of =)
+ assignment always go from left side to right side and not to another name

## Bookmark and Review

+ [Awesome Python Environment](https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5)

  + the python env - the interpretor, how to install, dependency management

+ [Python Module of the Week](https://pymotw.com/3/index.html)

  + This is a great cheatsheet!
