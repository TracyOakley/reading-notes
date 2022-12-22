# Class 4 Notes - Classes & Objects

[Back to Home](../README.md)

### [Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

+ class MyClass:
  + variable = "var"
  + def func(self):
    + print("Hello")
+ myobject = MyClass()
+ def __init__(self, number:)
  + self.number = number

### [Thinking Recursively in Python](https://realpython.com/python-thinking-recursively/)

+ Naively following the recursive deﬁnition of the nth Fibonacci number was rather inefficient. As you can see from the output above, we are unnecessarily recomputing values. Let’s try to improve fibonacci_recursive by caching the results of each Fibonacci computation Fk:
+ from functools import lru_cache

@lru_cache(maxsize=None)
def fibonacci_recursive(n):
    print("Calculating F", "(", n, ")", sep="", end=", ")

    # Base case
    if n == 0:
        return 0
    elif n == 1:
        return 1

    # Recursive case
    else:
        return fibonacci_recursive(n-1) + fibonacci_recursive(n-2)

+ lru_cache is a decorator that caches the results. Thus, we avoid recomputation by explicitly checking for the value before trying to compute it. One thing to keep in mind about lru_cache is that since it uses a dictionary to cache results, the positional and keyword arguments (which serve as keys in that dictionary) to the function must be hashable.

+ [Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

+ [Pytest Fixtures](https://docs.pytest.org/en/latest/explanation/fixtures.html)

+ In testing, a fixture provides a defined, reliable and consistent context for the tests. This could include environment (for example a database configured with known parameters) or content (such as a dataset).
+ Fixtures define the steps and data that constitute the arrange phase of a test (see Anatomy of a test). In pytest, they are functions you define that serve this purpose. They can also be used to define a test’s act phase; this is a powerful technique for designing more complex tests.
+ We can tell pytest that a particular function is a fixture by decorating it with @pytest.fixture. Here’s a simple example of what a fixture in pytest might look like:
+ @pytest.fixture
def my_fruit():
    return Fruit("apple")
+ Tests don’t have to be limited to a single fixture, either. They can depend on as many fixtures as you want, and fixtures can use other fixtures, as well. This is where pytest’s fixture system really shines.
