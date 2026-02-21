# Experiment 9- Study of Pandas Library

---

## Aim

To study the Pandas library in Python and perform data manipulation and analysis using Series and DataFrame structures.

---

## Objectives

* To understand the basics of the Pandas library
* To create and manipulate Series and DataFrames
* To perform data selection, filtering, and indexing
* To handle missing data
* To perform basic statistical analysis using Pandas
* To understand real-world applications of Pandas in data analysis

---

## Introduction to Pandas

Pandas is a powerful open-source Python library used for data analysis and data manipulation. It provides flexible and efficient data structures such as **Series** and **DataFrame**, which make handling structured data easy and intuitive.

Pandas is widely used in:

* Data Science
* Machine Learning
* Business Analytics
* Financial Analysis
* Research and Statistics
* Data Cleaning and Preprocessing

It is built on top of NumPy and allows fast operations on structured datasets.

---

## Theory

### 1. Pandas Series

A **Series** is a one-dimensional labeled array capable of holding data of any type (integer, string, float, etc.). Each element in a Series has an associated index.

Example:

```python
import pandas as pd

s = pd.Series([10, 20, 30, 40])
print(s)
```

---

### 2. Pandas DataFrame

A **DataFrame** is a two-dimensional labeled data structure with rows and columns. It is similar to a table in a database or an Excel spreadsheet.

Example:

```python
import pandas as pd

data = {
    "Name": ["A", "B", "C"],
    "Marks": [85, 90, 78]
}

df = pd.DataFrame(data)
print(df)
```

---

### 3. Important DataFrame Attributes

* `df.shape` → Returns number of rows and columns
* `df.columns` → Returns column names
* `df.index` → Returns row labels
* `df.dtypes` → Returns data types of columns
* `df.head()` → Displays first 5 rows
* `df.tail()` → Displays last 5 rows

---

### 4. Indexing and Selection

Pandas provides powerful indexing techniques:

* Selecting columns: `df["column_name"]`
* Selecting rows using `loc[]` (label-based indexing)
* Selecting rows using `iloc[]` (position-based indexing)

Example:

```python
print(df.loc[0])
print(df.iloc[1])
```

---

### 5. Handling Missing Data

Pandas provides functions to detect and handle missing values:

* `df.isnull()`
* `df.dropna()`
* `df.fillna()`

Handling missing data is important in real-world datasets to ensure accurate analysis.

---

### 6. Statistical Operations

Pandas allows quick statistical calculations:

* `df.mean()`
* `df.sum()`
* `df.max()`
* `df.min()`
* `df.describe()`

These functions help in understanding the dataset efficiently.

## Algorithm & Flowchart Additions 

### Program 1: Creating a Series

### Algorithm

1. Start
2. Import Pandas library
3. Create a Series using `pd.Series()`
4. Store it in a variable
5. Display the Series
6. Stop

### Flowchart

```id="p9s1f1"
Start
  ↓
Import Pandas
  ↓
Create Series using pd.Series()
  ↓
Store in variable
  ↓
Display Series
  ↓
Stop
```

---

## Program 2: Creating a DataFrame

### Algorithm

1. Start
2. Import Pandas library
3. Create a dictionary containing data
4. Convert dictionary into DataFrame using `pd.DataFrame()`
5. Store it in a variable
6. Display the DataFrame
7. Stop

### Flowchart

```id="p9s2f1"
Start
  ↓
Import Pandas
  ↓
Create Dictionary of Data
  ↓
Convert into DataFrame
  ↓
Store in variable
  ↓
Display DataFrame
  ↓
Stop
```

---

## Program 3: Data Selection

### Algorithm

1. Start
2. Import Pandas library
3. Create a DataFrame
4. Select a column using `df["column_name"]`
5. Select a row using `df.loc[]`
6. Display selected data
7. Stop

### Flowchart

```id="p9s3f1"
Start
  ↓
Import Pandas
  ↓
Create DataFrame
  ↓
Select Column
  ↓
Select Row using loc[]
  ↓
Display Selected Data
  ↓
Stop
```

---

## Program 4: Statistical Analysis

### Algorithm

1. Start
2. Import Pandas library
3. Create a DataFrame
4. Apply statistical functions such as:

   * `describe()`
   * `mean()`
   * `sum()`
5. Display results
6. Stop

### Flowchart

```id="p9s4f1"
Start
  ↓
Import Pandas
  ↓
Create DataFrame
  ↓
Apply Statistical Functions
  ↓
Display Results
  ↓
Stop
```

---

## Additional Algorithm: Handling Missing Data

### Algorithm

1. Start
2. Import Pandas library
3. Create or load a dataset
4. Check for missing values using `isnull()`
5. Handle missing values using:

   * `dropna()` to remove missing data
   * `fillna()` to replace missing data
6. Display updated dataset
7. Stop

---

## General Flow of a Pandas Program

```id="p9genf"
Start
  ↓
Import Pandas
  ↓
Create / Load Dataset
  ↓
Perform Data Manipulation
  ↓
Apply Analysis or Statistics
  ↓
Display Output
  ↓
Stop
```

## Sample Programs

### Program 1: Creating a Series

```python
import pandas as pd

series = pd.Series([5, 10, 15, 20])
print(series)
```

---

### Program 2: Creating a DataFrame

```python
import pandas as pd

data = {
    "Name": ["Rahul", "Sneha", "Amit"],
    "Age": [18, 19, 20]
}

df = pd.DataFrame(data)
print(df)
```

---

### Program 3: Data Selection

```python
print(df["Name"])
print(df.loc[0])
```

---

### Program 4: Statistical Analysis

```python
print(df.describe())
```

---

## Applications of Pandas

* Data cleaning and preprocessing
* Data visualization preparation
* Financial data analysis
* Machine learning data preparation
* Handling CSV and Excel files
* Large dataset analysis

---

## Advantages of Pandas

* Easy data handling and manipulation
* Powerful indexing and filtering
* Efficient handling of large datasets
* Integration with NumPy and Matplotlib
* Simplifies complex data operations

---

## Conclusion

The Pandas library is an essential tool for data analysis in Python. It simplifies the process of organizing, cleaning, analyzing, and manipulating structured data. Through this experiment, we learned how to create Series and DataFrames, perform indexing and filtering, handle missing values, and apply statistical functions effectively.

