# Experiment 19: COVID Data Analysis

---

## 1. Aim
To perform exploratory data analysis (EDA) on a COVID-19 dataset using Python to understand the spread, mortality, and recovery trends across different regions and time periods.

## 2. Introduction to Libraries Used
Effective data analysis requires tools that can handle large datasets and perform complex transformations. This experiment utilizes the following core Python libraries:

* **Pandas (`pd`):** The primary tool for data manipulation. It is used for loading datasets (CSV files), cleaning data (handling null values), and performing aggregations like grouping data by country or date.
* **NumPy (`np`):** Used for supporting high-level mathematical functions and multi-dimensional arrays, facilitating efficient numerical computations within the Pandas DataFrames.
* **Matplotlib/Seaborn/Plotly:** (As per the notebook's structure) These libraries are used to create visual representations of the COVID-19 trends, making the numerical data easier to interpret.

## 3. Common Utility Functions
Several essential functions are utilized during the data preprocessing and analysis phase:

* `pd.read_csv()`: Reads the raw dataset from a CSV file into a DataFrame.
* `data.head()`: Displays the first five rows of the dataset to provide a quick overview of the data structure.
* `data.drop(columns, axis)`: Removes unnecessary columns (e.g., 'SNo', 'Last Update') to streamline the analysis.
* `data.info()`: Provides a concise summary of the DataFrame, including the number of non-null entries and data types for each column.
* `astype()`: Converts data types of specific columns (e.g., converting 'ObservationDate' to datetime objects and 'Confirmed' to integers) for better computational performance.
* `fillna(value)`: Replaces missing or null values in the dataset with a specified value (e.g., 0) to prevent errors during calculation.

---

## 4. Step-by-Step Procedure and Plotting Functions

### Step 1: Data Loading and Initial Inspection
* **Action:** Load the `covid_19_data.csv` file and inspect its content.
* **Explanation:** The raw data is imported into a Pandas DataFrame. The `head()` and `info()` functions are used to identify columns like `ObservationDate`, `Country/Region`, `Confirmed`, `Deaths`, and `Recovered`.

### Step 2: Data Cleaning and Feature Engineering
* **Action:** Drop irrelevant columns and handle missing values.
* **Explanation:** Columns such as `SNo` and `Last Update` are removed using `data.drop()` as they do not contribute to the trend analysis. Missing values in the numerical columns (`Confirmed`, `Deaths`, `Recovered`) are filled with 0 to ensure the dataset is complete.
* **Feature Addition:** A new column, `Active`, is calculated by subtracting `Deaths` and `Recovered` from `Confirmed` cases to determine the number of current infections.

### Step 3: Type Casting for Analysis
* **Action:** Standardize data types.
* **Explanation:** The `ObservationDate` is converted to a standard `datetime64` format. This allows the analyst to perform time-series operations, such as grouping data by month or year to see the evolution of the pandemic.

### Step 4: Data Aggregation and Grouping
* **Action:** Group data by `ObservationDate` or `Country/Region`.
* **Explanation:** Using the `groupby()` function, the data is aggregated to find total global cases per day or total cases per country. This step is crucial for preparing the data for visualization.

### Step 5: Visualization of Trends
* **Action:** Generate charts to represent the spread of the virus.
* **Explanation:** * **Time-Series Line Charts:** Used to show the exponential growth of confirmed cases over time.
    * **Bar Charts:** Used to compare the total death tolls or recovery rates between different countries.
    * **Interactive Plots (Plotly):** (As indicated by the notebook metadata) Used to create dynamic graphs where users can hover over data points to see specific values for different regions.

---

## 5. Conclusion
The experiment demonstrates the complete pipeline of a data science project, from raw data ingestion and cleaning to advanced visualization. By transforming the COVID-19 dataset into structured formats and visual trends, we can effectively identify peak infection periods and compare the impact of the pandemic across various global regions.
<img width="4154" height="1216" alt="Image 17-04-26 at 2 43 PM" src="https://github.com/user-attachments/assets/df906d0e-31ac-4d99-b2ae-e8e6697e45bb" />
<img width="4148" height="1188" alt="Image 17-04-26 at 2 44 PM" src="https://github.com/user-attachments/assets/a563f344-ad20-4b8c-85ef-6731ce74b288" />
