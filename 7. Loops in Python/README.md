# **Experiment – 7**

## **Loops in Python**

## **Aim**

To study and implement looping statements in Python and understand repetition of statements using different loop constructs.


## **Objectives**

* To understand the concept of loops
* To implement `for` and `while` loops
* To use nested loops
* To apply loop control statements like `break`, `continue`, and `pass`
* To solve real-life programming problems using loops


## **Theory on Loops**

Loops in Python are used to execute a block of code repeatedly until a specified condition is satisfied. They help in reducing code repetition and making programs more efficient.

Python mainly provides two types of loops:

* `for` loop
* `while` loop

The `for` loop is generally used when the number of iterations is known in advance. It works with sequences like lists, tuples, strings, and ranges.

The `while` loop is used when the number of iterations depends on a condition. It runs as long as the condition remains `True`.

Python also provides loop control statements such as:

* `break` → Terminates the loop
* `continue` → Skips the current iteration
* `pass` → Acts as a placeholder

Indentation plays an important role in defining the scope of loops.


## **Types of Loops**

* `for` loop
* `while` loop
* Nested loops
* Loop control statements


# **Loop Algorithms**

## **Algorithm 1: Print Numbers from 1 to 5 (Using for Loop)**

1. Start
2. Use `range(1, 6)` to generate numbers from 1 to 5
3. Repeat for each number in the range
4. Print the number
5. Stop

---

## **Algorithm 2: Print Elements of a List**

1. Start
2. Create a list of numbers
3. Repeat for each element in the list
4. Print the element
5. Stop

---

## **Algorithm 3: Print Numbers from 1 to 5 (Using while Loop)**

1. Start
2. Initialize variable `i = 1`
3. Check if `i <= 5`
4. If true, print `i`
5. Increment `i` by 1
6. Repeat steps 3–5 until condition becomes false
7. Stop

---

## **Algorithm 4: Print Right-Angled Triangle Pattern**

1. Start
2. Use outer loop from 1 to 5
3. For each iteration of outer loop, run inner loop
4. Print `*` equal to current row number
5. Move to next line
6. Stop

---

## **Algorithm 5: Using break Statement**

1. Start
2. Run loop from 1 to 5
3. Check if number equals 3
4. If yes, terminate the loop using `break`
5. Otherwise, print the number
6. Stop

---

## **Algorithm 6: Using continue Statement**

1. Start
2. Run loop from 1 to 5
3. Check if number equals 3
4. If yes, skip current iteration using `continue`
5. Otherwise, print the number
6. Stop


## Program 1: Simple for Loop

```python
for i in range(1, 6):
    print(i)
```


## Program 2: for Loop with List

```python
numbers = [10, 20, 30, 40]

for num in numbers:
    print(num)
```


## Program 3: while Loop

```python
i = 1

while i <= 5:
    print(i)
    i += 1
```


## Program 4: Nested Loop (Right-Angled Triangle)

```python
for i in range(1, 6):
    for j in range(i):
        print("*", end="")
    print()
```

## Program 5: Loop Control Statements

### Using break

```python
for i in range(1, 6):
    if i == 3:
        break
    print(i)
```

### Using continue

```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```


## **Applications of Loops**

* Printing patterns
* Iterating through lists and strings
* Calculating sums and averages
* Checking prime numbers
* Menu-driven programs
* Repetitive real-life tasks


## **Conclusion**

Loops are essential in Python programming as they allow repetitive execution of code efficiently. By using `for`, `while`, nested loops, and loop control statements, programmers can solve complex problems in a structured and simplified manner. Mastering loops is fundamental for developing logical and efficient programs.
