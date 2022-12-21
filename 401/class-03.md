# Class 3 Notes - FileIO & Exceptions

[Back to Home](../README.md)

### [Read & Write File in Python](https://realpython.com/read-write-files-python/)

+ Files are a contiguous set of bytes used to store data.
+ Files are made of Header, Data, End of File
+ Python: open() to open a file (Remember to close)
+ reader = open('dog_breeds.txt')
  + try:
  + Further file processing goes here
  + finally:
  + reader.close()
+ OR USE with open('dog_breeds.txt') as reader:

### [Exceptions in Python](https://realpython.com/python-exceptions/)

+ A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception. 
+ an exception error. This type of error occurs whenever syntactically correct Python code results in an error. The last line of the message indicated what type of exception error you ran into.
+ Raising an Exception, Assertion Error, Handling Errors
+ Try, Except, else, finally
+ raise allows you to throw an exception at any time.
+ assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
+ In the try clause, all statements are executed until an exception is encountered.
except is used to catch and handle the exception(s) that are encountered in the try clause.
+ else lets you code sections that should run only when no exceptions are encountered in the try clause.
+ finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

### [Read and Write Files in Python - Video](https://realpython.com/courses/reading-and-writing-files-python/)


### [Reading and Writing Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)
