**Experiment - 5**

**Title**

**Implementation of Set and Dictionary in Python**

**Aim**

To study and implement set data structure in Python and perform various set and Dictionary operations.

**Objectives**

- To understand the concept of sets
- To perform set creation and basic operations
- To apply mathematical set operations
- To understand dictionary structure
- To perform insertion, deletion, and access of data
- To apply dictionary methods

**Theory on Sets**
A set in Python is an unordered collection of unique elements. Sets are defined using curly braces {} or the set() constructor. Since sets do not allow duplicate values, they are useful for handling distinct data efficiently.

Sets are mutable, meaning elements can be added or removed after creation. However, sets do not support indexing due to their unordered nature.

**Characteristics of Set**

- Unordered
- No duplicate elements
- Mutable
- Does not support indexing

Sets are commonly used in real-life scenarios such as **removing duplicates**, **membership testing**, and **mathematical operations**.

**Set Operations**

- Union
- Intersection
- Difference
- Symmetric Difference

**Program 1: Creating a Set and Displaying Elements**

fruits = {"apple", "banana", "cherry"}

print("Fruits:", fruits)

**Program 2: Removing Duplicate Values**

numbers = {1, 2, 3, 2, 4, 1}

print("Unique numbers:", numbers)

**Program 3: Set Operations**

A = {1, 2, 3, 4}

B = {3, 4, 5, 6}

print("Union:", A | B)

print("Intersection:", A & B)

print("Difference:", A - B)

print("Symmetric Difference:", A ^ B)

**Program 4: Set Methods**

s = {10, 20, 30}

s.add(40)

s.remove(20)

print("Updated Set:", s)

**Applications of Set**

- Removing duplicate records
- Membership testing
- Mathematical computations

**Theory on dictionary**

A dictionary is an unordered collection of key–value pairs where each key must be unique. Dictionaries are defined using curly braces with keys and values separated by a colon.
Dictionaries are mutable and allow insertion, deletion, and modification of data. Values can be accessed quickly using their corresponding keys, making dictionaries efficient for data storage and retrieval.

Syntax:

dictionary = {key: value}

Dictionaries are widely used in real-life applications such as **student records**, **phone books**, and **configuration data**.

**Characteristics of Dictionary**

- Key-value based
- Mutable
- Keys are unique
- Values can be modified

**Program 1: Creating and Accessing Dictionary**

student = {

"roll": 101,

"name": "Amit",

"branch": "CSE"

}

print("Name:", student\["name"\])

**Program 2: Adding and Updating Elements**

student\["year"\] = "Second"

student\["name"\] = "Rahul"

print(student)

**Program 3: Removing Elements**

student.pop("branch")

print("After removal:", student)

**Program 4: Dictionary Methods**

print("Keys:", student.keys())

print("Values:", student.values())

print("Items:", student.items())

**Program 5: Iterating Through Dictionary**

for key, value in student.items():

print(key, ":", value)

**Applications of Dictionary**

- Student information systems
- Phone directories
- Database records
- Configuration files

**Conclusion**
Sets efficiently manage unique data and support mathematical operations, while dictionaries provide fast and organized storage of data using key–value pairs, making both structures essential in Python programming.
