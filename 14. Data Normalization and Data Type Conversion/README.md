# Experiment 14: Data Normalization and Encoding of Categorical Variables in Python

---

## Aim

To study and implement data preprocessing techniques using Python. The experiment focuses on normalization methods and encoding of categorical variables using Pandas and Scikit-learn.

---

## Introduction

In real-world data analysis and machine learning tasks, raw data is often inconsistent and not directly suitable for modeling. Data preprocessing is an essential step to clean, transform, and prepare the data.

Two important preprocessing techniques are:

1. Data Normalization:
   Numerical features often have different ranges. For example, product prices may be in thousands, while ratings lie between 1 and 5. Without normalization, larger values dominate the model. Normalization scales features into a comparable range.

2. Encoding Categorical Variables:
   Machine learning models require numerical input. Categorical values such as gender or department must be converted into numeric form using encoding techniques.

---

## Libraries Used

Pandas:
Used for data manipulation and handling tabular data through DataFrames.

NumPy:
Provides numerical operations such as mean, standard deviation, and array calculations.

Scikit-learn:
Provides preprocessing tools like LabelEncoder for converting categorical values into numbers.

---

## Preprocessing Techniques

### Part A: Data Normalization

Min-Max Normalization:
Rescales values to a fixed range between 0 and 1.
Formula: (x - min) / (max - min)

Z-Score Normalization:
Standardizes data to have mean 0 and standard deviation 1.
Formula: (x - mean) / standard deviation

Decimal Scaling:
Scales values by dividing them by a power of 10.
Formula: x / (10^k)

Multi-column normalization:
Applies normalization to multiple columns simultaneously using vectorized operations.

---

### Part B: Encoding Categorical Variables

Label Encoding:
Assigns a unique integer value to each category. Suitable for binary or ordered categories.

One-Hot Encoding:
Creates separate binary columns for each category. Suitable for categorical variables without any order.

Dummy Encoding:
Similar to One-Hot Encoding but removes one column to avoid redundancy in regression models.

---

## Key Functions Used

| Function / Command              | Library               | Purpose                      |
| ------------------------------- | --------------------- | ---------------------------- |
| pd.DataFrame()                  | Pandas                | Create DataFrame from data   |
| pd.read_csv()                   | Pandas                | Load dataset from CSV file   |
| df.min()                        | Pandas                | Find minimum value           |
| df.max()                        | Pandas                | Find maximum value           |
| df.mean()                       | Pandas                | Calculate average            |
| df.std()                        | Pandas                | Calculate standard deviation |
| pd.get_dummies()                | Pandas                | Perform One-Hot Encoding     |
| pd.get_dummies(drop_first=True) | Pandas                | Perform Dummy Encoding       |
| LabelEncoder()                  | sklearn.preprocessing | Create label encoder         |
| fit()                           | sklearn               | Learn parameters             |
| transform()                     | sklearn               | Apply transformation         |
| fit_transform()                 | sklearn               | Learn + apply transformation |
---

## Procedure

### Part A: Normalization

1. Import Pandas and NumPy libraries.
2. Create a dataset using a dictionary.
3. Apply Min-Max normalization to selected columns.
4. Apply Z-Score normalization to numerical data.
5. Perform Decimal Scaling.
6. Normalize multiple columns together.
7. Load external dataset using CSV and repeat steps.
8. Verify results.

### Part B: Encoding

1. Create a dataset containing categorical variables.
2. Apply Label Encoding to binary columns.
3. Perform One-Hot Encoding on nominal columns.
4. Apply Dummy Encoding using drop_first=True.
5. Load student dataset and apply encoding techniques.
6. Verify outputs.

---

## Dataset Description

Product Dataset
Contains Product, Price, Units_Sold, and Discount.
Used to demonstrate normalization techniques.

Amazon Dataset
Contains product details such as Product_ID, Price, Rating, Reviews, and Units_Sold.
Used for real-world normalization.

Orders Dataset
Contains Order ID, Gender, Payment Method, Category, City, and Order Value.
Used for encoding techniques.

Student Dataset
Contains student academic and placement information such as Department, CGPA, and Placement Status.
Used for encoding categorical variables.

---

## Applications

* E-commerce recommendation systems
* Banking and financial analysis
* Healthcare prediction systems
* Student placement analysis
* Natural language processing
* Computer vision models

---

## Conclusion

This experiment demonstrated how normalization and encoding techniques are used to prepare data for machine learning models.

Normalization ensures that all numerical features are on a similar scale, preventing bias in models. Encoding converts categorical data into numerical form so that algorithms can process it.

Selecting the appropriate method depends on the type of data and the requirements of the model.

---

## Additional Notes

Label Encoding vs One-Hot Encoding
Label encoding is suitable for binary or ordered data. One-Hot encoding is preferred for nominal data without any order.

Dummy Variable Trap
Using all One-Hot encoded columns can create redundancy. Dropping one column avoids this issue.

fit(), transform(), fit_transform()
fit() learns parameters
transform() applies transformation
fit_transform() performs both steps together


## Normalization Guide

| Situation                        | Technique       |
| -------------------------------- | --------------- |
| Need values between 0 and 1      | Min-Max         |
| Data follows normal distribution | Z-Score         |
| Quick scaling required           | Decimal Scaling |
| Tree-based models                | Not required    |

---
