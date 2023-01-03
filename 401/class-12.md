# Class 12 Notes - Pandas

[Back to Home](../README.md)

### [Pandas in 10 minutes](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

+ import numpy as np
+ import pandas as pd
+ Creating a Series by passing a list of values, letting pandas create a default integer index:
  + s = pd.Series([1, 3, 5, np.nan, 6, 8])
+ Viewing Data
  + Use DataFrame.head() and DataFrame.tail() to view the top and bottom rows of the frame respectively:
+ DataFrame.to_numpy() gives a NumPy representation of the underlying data. Note that this can be an expensive operation when your DataFrame has columns with different data types, which comes down to a fundamental difference between pandas and NumPy: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column. When you call DataFrame.to_numpy(), pandas will find the NumPy dtype that can hold all of the dtypes in the DataFrame. This may end up being object, which requires casting every value to a Python object.

### [Pandas - Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)

+ import pandas as pd
+ df = pd.DataFrame({...
+ To manually store data in a table, create a DataFrame. When using a Python dictionary of lists, the dictionary keys will be used as column headers and the values in each list as columns of the DataFrame.
+ A DataFrame is a 2-dimensional data structure that can store data of different types (including characters, integers, floating point values, categorical data and more) in columns. It is similar to a spreadsheet, a SQL table or the data.frame in R.

### [Real Python - Pandas Tutorials](https://realpython.com/learning-paths/pandas-data-science/)

+ Pandas is a game-changer for data science and analytics, particularly if you came to Python because you were searching for something more powerful than Excel and VBA. Pandas uses fast, flexible, and expressive data structures designed to make working with relational or labeled data both easy and intuitive.

### [What is Pandas - Video](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)

### [Master Pandas - Bookmark](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)
