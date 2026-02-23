# Experiment 8
# Tools in EDA: Study of NumPy Library

## Aim

To study the NumPy library in Python and implement various numerical operations using NumPy arrays and built-in functions.


## Objectives

* To understand the concept of NumPy arrays
* To create and manipulate one-dimensional and multi-dimensional arrays
* To perform mathematical and statistical operations using NumPy
* To understand array indexing, slicing, reshaping, and broadcasting
* To apply NumPy functions in real-life numerical computations


## Introduction to NumPy

NumPy (Numerical Python) is a fundamental library in Python used for scientific computing and numerical analysis. It provides support for large, multi-dimensional arrays and matrices along with a collection of high-level mathematical functions to operate on these arrays efficiently.

NumPy is widely used in:

* Data Science
* Machine Learning
* Artificial Intelligence
* Scientific Research
* Data Analytics
* Engineering computations

It is faster and more memory-efficient than Python lists because it is implemented in C and performs operations using optimized vectorized code.

---

## Theory

### 1. NumPy ndarray (N-Dimensional Array)

The core data structure in NumPy is the **ndarray**. It represents a grid of values, all of the same data type, and is indexed using integers.

Key characteristics of ndarray:

* Homogeneous data type (all elements are of the same type)
* Fixed size once created
* Faster numerical operations compared to lists
* Supports vectorized operations

Example:

```python
import numpy as np
arr = np.array([1, 2, 3, 4])
```

---

### 2. Array Attributes

NumPy arrays have several important attributes:

* `arr.ndim` → Number of dimensions
* `arr.shape` → Shape of the array (rows, columns)
* `arr.size` → Total number of elements
* `arr.dtype` → Data type of elements

These attributes help in understanding and manipulating the structure of arrays.

---

### 3. Array Creation Methods

NumPy provides multiple ways to create arrays:

* `np.array()` → Create array from list/tuple
* `np.zeros()` → Create array filled with zeros
* `np.ones()` → Create array filled with ones
* `np.arange()` → Create array within a range
* `np.linspace()` → Create evenly spaced values
* `np.random.rand()` → Generate random values

---

### 4. Indexing and Slicing

NumPy supports powerful indexing and slicing techniques:

* Access single elements
* Extract rows and columns
* Slice specific portions of arrays

Example:

```python
arr = np.array([10, 20, 30, 40])
print(arr[1:3])
```

---

### 5. Mathematical Operations

NumPy allows element-wise operations without using loops:

* Addition, subtraction, multiplication, division
* Square root, power, exponential functions
* Trigonometric functions

Example:

```python
arr = np.array([1, 2, 3])
print(arr * 2)
```

---

### 6. Broadcasting

Broadcasting allows NumPy to perform operations on arrays of different shapes. It automatically adjusts smaller arrays to match the shape of larger arrays during operations.

This feature eliminates the need for manual looping and improves efficiency.

---

### 7. Reshaping Arrays

Using `reshape()`, arrays can be converted into different dimensions without changing the data.

Example:

```python
arr = np.arange(6)
reshaped = arr.reshape(2, 3)
```

## Applications of NumPy

* Mathematical computations
* Matrix operations
* Statistical analysis
* Image processing
* Machine learning model development
* Handling large datasets efficiently
* Scientific simulations

## Advantages of NumPy

* Faster execution compared to Python lists
* Efficient memory usage
* Supports multi-dimensional arrays
* Built-in optimized mathematical functions
* Enables vectorized operations
* Easily integrates with libraries like Pandas, Matplotlib, and Scikit-learn


## Conclusion

The NumPy library plays a vital role in numerical and scientific computing in Python. It provides powerful tools for handling arrays, performing mathematical operations, reshaping data, and implementing efficient computations. Through this experiment, we gained practical knowledge of array creation, manipulation, and application of NumPy functions in real-world scenarios.

