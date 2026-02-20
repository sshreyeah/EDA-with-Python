# Experiment – 8 
# Study of NumPy Library

## Aim

To study the NumPy library in Python and implement various numerical operations using NumPy arrays and built-in functions.


## Objectives

* To understand the concept of NumPy arrays
* To create and manipulate one-dimensional and multi-dimensional arrays
* To perform mathematical and statistical operations using NumPy
* To understand array indexing, slicing, and reshaping
* To apply NumPy functions in real-life numerical computations


## Introduction to NumPy

NumPy (Numerical Python) is a powerful Python library used for numerical computing. It provides support for large, multi-dimensional arrays and matrices, along with a wide collection of mathematical functions to operate on these arrays efficiently.

NumPy is widely used in:

* Data Science
* Machine Learning
* Scientific Computing
* Artificial Intelligence
* Data Analysis

It is faster and more efficient than Python lists for numerical operations because it is implemented in C and optimized for performance.


## Theory

### 1. NumPy Arrays

The core object of NumPy is the **ndarray (N-dimensional array)**. It is a grid of values, all of the same type, indexed by a tuple of non-negative integers.

Example:

```python
import numpy as np

arr = np.array([1, 2, 3, 4])
```


### 2. Types of Arrays

* **1-D Array** – Single row of elements
* **2-D Array** – Matrix (rows and columns)
* **Multi-Dimensional Array** – Higher dimensional arrays

---

### 3. Important NumPy Functions

* `np.array()` – Create an array
* `np.zeros()` – Create array filled with zeros
* `np.ones()` – Create array filled with ones
* `np.arange()` – Create array with a range of values
* `np.reshape()` – Change the shape of array
* `np.sum()` – Find sum of elements
* `np.mean()` – Calculate mean
* `np.max()` / `np.min()` – Find maximum/minimum value


## Sample Programs

### Program 1: Creating a NumPy Array

```python
import numpy as np

arr = np.array([10, 20, 30, 40])
print("Array:", arr)
```


### Program 2: Creating a 2-D Array

```python
import numpy as np

matrix = np.array([[1, 2, 3], [4, 5, 6]])
print("2D Array:\n", matrix)
```


### Program 3: Array Operations

```python
import numpy as np

arr = np.array([1, 2, 3, 4])

print("Sum:", np.sum(arr))
print("Mean:", np.mean(arr))
print("Maximum:", np.max(arr))
```


### Program 4: Reshaping an Array

```python
import numpy as np

arr = np.arange(6)
reshaped = arr.reshape(2, 3)

print("Original Array:", arr)
print("Reshaped Array:\n", reshaped)
```


## Applications of NumPy

* Mathematical computations
* Matrix operations
* Statistical analysis
* Image processing
* Machine learning model development
* Handling large datasets efficiently

## Advantages of NumPy

* Faster execution compared to Python lists
* Efficient memory usage
* Supports multi-dimensional arrays
* Provides built-in mathematical functions
* Easy integration with other libraries like Pandas and Matplotlib

---

## Conclusion

The NumPy library is an essential tool for numerical and scientific computing in Python. It simplifies complex mathematical operations and improves computational efficiency. Through this experiment, we understood how to create arrays, perform operations, reshape data, and apply statistical functions using NumPy.
