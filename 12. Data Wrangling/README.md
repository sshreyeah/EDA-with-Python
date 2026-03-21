# **Experiment 12 – Data Wrangling Using Python**

## **Aim**

To perform data wrangling using Python and the Pandas library by cleaning, transforming, and preparing raw data for analysis.

---

## **Objectives**

* To understand the concept of data wrangling
* To handle missing and inconsistent data
* To clean and preprocess datasets using Pandas
* To transform data into a suitable format for analysis
* To rename, modify, and restructure data columns
* To filter and sort datasets effectively
* To merge and combine multiple datasets

---

## **Introduction**

Data wrangling, also known as data cleaning or data preprocessing, is the process of transforming raw data into a clean and structured format suitable for analysis.

In real-world datasets, data is often incomplete, inconsistent, or contains errors. Data wrangling helps improve data quality by handling missing values, correcting inconsistencies, and formatting data properly.

Python provides powerful libraries such as Pandas that make data wrangling efficient and easy. Using Pandas, analysts can clean, transform, and organize data before performing analysis or visualization.

Data wrangling is widely used in data science, machine learning, business analytics, and research.

---

## **Theory**

### **1. Data Wrangling**

Data wrangling involves cleaning, transforming, and organizing data to make it suitable for analysis.

Key steps include:

* Handling missing values
* Removing duplicates
* Formatting data
* Filtering and sorting
* Merging datasets

---

### **2. Handling Missing Values**

Missing data can affect analysis accuracy. Pandas provides methods to handle missing values:

* `isnull()` – Detect missing values
* `dropna()` – Remove missing values
* `fillna()` – Replace missing values

Example:

```python
df.isnull()
df.dropna()
df.fillna(0)
```

---

### **3. Removing Duplicates**

Duplicate data can lead to incorrect analysis.

* `duplicated()` – Identifies duplicates
* `drop_duplicates()` – Removes duplicate rows

Example:

```python
df.drop_duplicates()
```

---

### **4. Data Transformation**

Data transformation modifies data into a usable format.

Examples include:

* Changing data types
* Creating new columns
* Applying functions

Example:

```python
df['Price'] = df['Price'].astype(int)
df['Total'] = df['Quantity'] * df['Price']
```

---

### **5. Renaming Columns**

Column names can be modified for better readability.

Example:

```python
df.rename(columns={'old_name':'new_name'}, inplace=True)
```

---

### **6. Filtering Data**

Filtering extracts specific data based on conditions.

Example:

```python
df[df['Category'] == 'Technology']
```

---

### **7. Sorting Data**

Sorting arranges data in a meaningful order.

Example:

```python
df.sort_values(by='Price')
```

---

### **8. Merging and Joining Data**

Combining multiple datasets is an important step in data wrangling.

Example:

```python
pd.merge(df1, df2, on='ID')
```

---

## **Algorithms**

### **Algorithm 1: Handling Missing Values**

Start
Import Pandas library
Load dataset
Check for missing values using `isnull()`
Handle missing values using `dropna()` or `fillna()`
Display cleaned dataset
Stop

---

### **Algorithm 2: Removing Duplicates**

Start
Load dataset
Check duplicate rows using `duplicated()`
Remove duplicates using `drop_duplicates()`
Display dataset
Stop

---

### **Algorithm 3: Data Transformation**

Start
Load dataset
Select required columns
Apply transformations (type conversion, new columns)
Display updated dataset
Stop

---

### **Algorithm 4: Filtering and Sorting Data**

Start
Load dataset
Apply filtering condition
Sort data using `sort_values()`
Display results
Stop

---

## **Sample Code Snippets**

### **Loading Dataset**

```python
import pandas as pd

df = pd.read_csv("data.csv")
print(df)
```

---

### **Handling Missing Values**

```python
print(df.isnull())
df = df.fillna(0)
```

---

### **Removing Duplicates**

```python
df = df.drop_duplicates()
```

---

### **Data Transformation**

```python
df['Total'] = df['Quantity'] * df['Price']
```

---

### **Filtering Data**

```python
print(df[df['Category'] == 'Furniture'])
```

---

### **Sorting Data**

```python
print(df.sort_values(by='Price'))
```

---

### **Merging Data**

```python
df3 = pd.merge(df1, df2, on='ID')
```

---

## **Applications**

* Data preprocessing for machine learning
* Business data cleaning and reporting
* Financial data analysis
* Customer data preparation
* Survey and research data cleaning
* Data integration from multiple sources

---

## **Advantages**

* Improves data quality and accuracy
* Handles missing and inconsistent data effectively
* Prepares data for analysis and visualization
* Saves time in data preprocessing
* Integrates well with analysis and ML tools

---

## **Result**

Data wrangling was successfully performed using Python and the Pandas library. Various operations such as handling missing values, removing duplicates, transforming data, filtering, sorting, and merging datasets were carried out to clean and prepare the dataset for further analysis.

