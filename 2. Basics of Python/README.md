# **EXPERIMENT – 2**
---

## **TITLE**
**Study of Python Programming Environment, Data Types, Operators, and Basic Input/Output**
---

## **AIM**
To study the Python programming environment and interface, understand execution modes, comments, variables, data types, operators, and basic input/output operations using a single integrated Python program.
---

## **THEORY**
Python is a high-level, interpreted programming language that supports multiple programming paradigms.  
A Python program can be executed in **Interactive Mode** or **Script Mode**.

- **Interactive Mode** executes one statement at a time and displays immediate output.
- **Script Mode** executes a complete program saved in a `.py` file.

Python supports:
- **Comments** for documentation
- **Variables** for storing data dynamically
- **Built-in data types** such as integer, float, string, and boolean
- **Operators** for arithmetic, relational, logical, assignment, and bitwise operations
- **Input and Output functions** to interact with users

This experiment demonstrates all the above concepts in a single consolidated Python program.
---

## **PROGRAM (COMBINED CODE)**
```python
# -------------------------------
# Python Basics Demonstration
# -------------------------------

"""
This program demonstrates:
- Comments
- Variables and data types
- Operators
- Input and Output
"""

print("WELCOME TO PYTHON PROGRAMMING")

# Variables and Data Types
name = "Snehal"
age = 45
height = 5.3
is_faculty = True

print("\n--- Data Types ---")
print("Name:", name, type(name))
print("Age:", age, type(age))
print("Height:", height, type(height))
print("Faculty:", is_faculty, type(is_faculty))

# Operators
a = 10
b = 5

print("\n--- Arithmetic Operators ---")
print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)

print("\n--- Relational Operators ---")
print("a > b:", a > b)
print("a == b:", a == b)

print("\n--- Logical Operators ---")
print("AND:", a > 5 and b > 2)
print("OR:", a > 20 or b > 2)
print("NOT:", not(a > b))

print("\n--- Assignment Operator ---")
c = a
c += b
print("c =", c)

print("\n--- Bitwise Operators ---")
print("Bitwise AND:", a & b)
print("Bitwise OR:", a | b)

# Input and Output
print("\n--- Input and Output ---")
student_name = input("Enter student name: ")
marks = int(input("Enter marks: "))

print("Student Name:", student_name)
print("Marks Obtained:", marks)

## **CONCLUSION**
Thus, the Python programming environment, execution modes, comments, variables, data types, operators, and basic
input/output operations were successfully studied and implemented using a single integrated Python program.
