# Experiment–4  
## Tuples in Python: Creation, Access, and Operations

### Aim
To understand Python tuples and perform operations such as creation, indexing, slicing, unpacking, and using built-in functions.

### Objectives
- Understand the concept of tuples in Python  
- Study characteristics and advantages of tuples  
- Perform indexing and slicing operations  
- Apply built-in tuple functions  
- Understand the immutability of tuples  

### Theory

#### 1. Introduction to Tuples
A **tuple** is an ordered collection of elements in Python, similar to a list, but **immutable** in nature. Once created, the elements of a tuple cannot be modified. Tuples are written using parentheses `()` and elements are separated by commas.

**Example:**  
`(10, 20, 30)`

#### 2. Characteristics of Tuples
Tuples have the following properties:
- **Ordered:** Elements maintain insertion order  
- **Indexed:** Index starts from 0  
- **Immutable:** Elements cannot be changed after creation  
- **Allows Duplicates:** Same value can appear multiple times  
- **Heterogeneous:** Can store different data types  

#### 3. Uses and Advantages of Tuples
Tuples are preferred when:
- Data should not be modified (data integrity)  
- Faster access is required compared to lists  
- Representing fixed data such as coordinates, days of the week, or database records  

#### 4. Creating Tuples
Tuples can be created in multiple ways:
- Using parentheses  
- Without parentheses (tuple packing)  
- Using the `tuple()` constructor  

**Special Case:**  
A single-element tuple must include a trailing comma:  
`(10,)`

#### 5. Indexing in Tuples
Tuple elements can be accessed using index numbers.
- **Positive indexing:** Left to right (0, 1, 2, …)  
- **Negative indexing:** Right to left (-1, -2, …)  

Indexing is used to retrieve specific elements from a tuple.

#### 6. Slicing in Tuples
Slicing extracts a portion of a tuple and returns a new tuple.

**Syntax:**  
`tuple_name[start : end : step]`

- `start` – starting index (included)  
- `end` – ending index (excluded)  
- `step` – interval between elements  

Slicing does not modify the original tuple.

#### 7. Immutability of Tuples
Tuples are immutable, meaning:
- Elements cannot be added  
- Elements cannot be removed  
- Elements cannot be updated  

Any attempt to modify a tuple results in an error.

#### 8. Built-in Functions for Tuples
Common functions used with tuples include:

| Function | Description |
|--------|-------------|
| `len()` | Returns number of elements |
| `max()` | Returns maximum value |
| `min()` | Returns minimum value |
| `sum()` | Returns sum of elements |
| `count()` | Counts occurrences of an element |
| `index()` | Returns index of an element |

#### 9. Difference Between List and Tuple

| List | Tuple |
|-----|-------|
| Mutable | Immutable |
| Uses `[ ]` | Uses `( )` |
| Slower | Faster |
| Dynamic | Fixed |

### Programs Included
- Student exam result using tuple unpacking  
- Employee attendance analysis using tuple methods  

### Conclusion
Python tuples provide a secure and efficient way to store fixed data. Their immutability, fast access, and support for indexing, slicing, and built-in functions make them suitable for representing constant and structured data.
