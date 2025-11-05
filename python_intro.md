# Python Introduction

## 1.Print Statment
### what is print statement in python?

>In Python, the print() statement is used to display output on the screen.

#### Syntax
```
print(object, sep=' ', end='\n', file=sys.stdout, flush=False)
```
#### Example
```
print("Hello, World!")
```
#### Output
Hello, World!

---
## 2.Comments in python
### what is comments line in python and it's type?
>A comment in Python is a piece of text that starts with the # symbol and is not executed by the Python interpreter.

### Types
#### 1. Single-line comment
Starts with a # symbol — anything after # on that line is ignored.

#### Example
```
# This is a single-line comment
print("Hello, World!")  # This prints a message
```
#### output

Hello, World!

### 2. Multi-line comment
Python doesn’t have a dedicated multi-line comment syntax,
but we can use triple quotes (''' or """) to write multi-line comments.

#### Example
```
'''
This is a multi-line comment.
You can use it to describe your code
in detail.
'''
print("Python Comments Example")
```
#### output

Python Comments Example

### why use comments?
To **describe** what your code does

To make **debugging easier**

To **temporarily disable** lines of code

To **improve readability** for others (and your future self)

---
## 3. Data Types
In Python, data types tell the interpreter what kind of value a variable holds — like a number, text, list, etc.

| **Category**           | **Data Type** | **Description / Summary**                         | **Example**                             |
| ---------------------- | ------------- | ------------------------------------------------- | --------------------------------------- |
| **1️⃣ Numeric Types**  | `int`         | Integer numbers (no decimals)                     | `x = 10`                                |
|                        | `float`       | Decimal or floating-point numbers                 | `y = 10.5`                              |
|                        | `complex`     | Complex numbers (a + bj)                          | `z = 3 + 5j`                            |
| **2️⃣ Sequence Types** | `str`         | String (collection of characters in quotes)       | `name = "Python"`                       |
|                        | `list`        | Ordered, changeable collection of items           | `numbers = [1, 2, 3]`                   |
|                        | `tuple`       | Ordered, **unchangeable** collection of items     | `point = (10, 20)`                      |
| **3️⃣ Mapping Type**   | `dict`        | Key-value pairs (like a real dictionary)          | `student = {"name": "John", "age": 21}` |
| **4️⃣ Set Types**      | `set`         | Unordered, unique items only                      | `colors = {"red", "green", "blue"}`     |
|                        | `frozenset`   | Same as set but **immutable (cannot be changed)** | `fset = frozenset({1, 2, 3})`           |
| **5️⃣ Boolean Type**   | `bool`        | Logical values — `True` or `False`                | `flag = True`                           |
| **6️⃣ Binary Types**   | `bytes`       | Sequence of bytes (immutable)                     | `b = b"Hello"`                          |
|                        | `bytearray`   | Mutable sequence of bytes                         | `ba = bytearray([65, 66, 67])`          |
|                        | `memoryview`  | Memory view of bytes (advanced)                   | `mv = memoryview(b"abc")`               |
| **7️⃣ None Type**      | `NoneType`    | Represents the absence of value                   | `x = None`                              |

### Example
```
# Numeric
a = 10          # int
b = 10.5        # float
c = 2 + 3j      # complex

# Sequence
name = "Python" # str
numbers = [1, 2, 3] # list
coords = (10, 20)   # tuple

# Mapping
student = {"name": "Bhuvan", "age": 22}

# Set
colors = {"red", "blue"}

# Boolean
is_active = True

# None
x = None
```
### Summary
| **Category** | **Purpose**                                       |
| ------------ | ------------------------------------------------- |
| **Numeric**  | Store numbers (whole, decimal, or complex)        |
| **Sequence** | Store ordered collections (text or list of items) |
| **Mapping**  | Store data as key–value pairs                     |
| **Set**      | Store unique, unordered items                     |
| **Boolean**  | Store truth values (`True` / `False`)             |
| **Binary**   | Store byte data (for files, images, etc.)         |
| **None**     | Represent “no value” or “empty”                   |

---
## 4. Variables
Variables are **containers** for storing data **values.**

A variable is a **name** used to store a **value** in memory.
### Rules for Python variables
A variable name must start with a letter or the underscore character

A variable name cannot start with a number

A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )

Variable names are case-sensitive (age, Age and AGE are three different variables)

A variable name cannot be any of the Python keywords.

| Rule                                                                | Example                         |
| ------------------------------------------------------------------- | ------------------------------- |
| 1️⃣ Variable names must start with a **letter or underscore (`_`)** | ✅ `_name`, `age`                |
| 2️⃣ Cannot start with a **number**                                  | ❌ `1name`                       |
| 3️⃣ Can contain **letters, numbers, and underscores**               | ✅ `student_1`, `marks_count`    |
| 4️⃣ Are **case-sensitive**                                          | `Age` and `age` are different   |
| 5️⃣ Should not use **Python keywords**                              | ❌ `if`, `while`, `for`, `class` |

---
## 5. Keywords in Python
🔹 Keywords are special reserved words in Python that have a specific meaning and purpose.

🔹 You cannot use them as variable names, function names, or identifiers.

🔹 They define the syntax and structure of the Python language.

### example
```
if = 5      # ❌ Error — 'if' is a keyword
```
### List of All Python Keywords (Python 3.11 / 3.12)
| Category               | Keywords                                       | Meaning / Usage                  |
| ---------------------- | ---------------------------------------------- | -------------------------------- |
| **Control Flow**       | `if`, `elif`, `else`                           | Conditional statements           |
|                        | `for`, `while`, `break`, `continue`, `pass`    | Loops and control flow           |
| **Functions**          | `def`, `return`, `yield`, `lambda`             | Define and return from functions |
| **Classes & Objects**  | `class`, `self`, `del`                         | Object-oriented programming      |
| **Boolean & None**     | `True`, `False`, `None`                        | Boolean values and null value    |
| **Logical Operators**  | `and`, `or`, `not`, `in`, `is`                 | Logical and identity operations  |
| **Exception Handling** | `try`, `except`, `finally`, `raise`, `assert`  | Error handling                   |
| **Importing Modules**  | `import`, `from`, `as`                         | Module management                |
| **Variable Scope**     | `global`, `nonlocal`                           | Define variable scope            |
| **Async Programming**  | `async`, `await`                               | Asynchronous programming         |
| **Other Keywords**     | `with`, `yield`, `breakpoint`, `match`, `case` | Special use cases                |

### View all keywords
```
import keyword
print(keyword.kwlist)
```
## 6. Control Statements
A control statement in Python is used to control the flow of execution of a program —
that means deciding which part of the code should run and when.

### Types of Control Statements
<p align="center">
if

else

elif
</p>

### 6.1 if Statement:

The if statement is a decision-making statement.

It allows your program to execute a block of code only if a certain condition is true.

#### Syntax
<p align="center">
<img width="369" height="103" alt="image" src="https://github.com/user-attachments/assets/8519d604-3e40-4861-ae78-0cff6c9ebf9f" />
</p>


#### Example
```
age = 20

if age >= 18:
    print("You are eligible to vote.")
```
### 6.2 if...else Statement
Used when you want to do one thing if the condition is true, and something else if it’s false.

#### Syntax

<p align="center">
<img width="433" height="154" alt="image" src="https://github.com/user-attachments/assets/b67754c8-2306-4e06-bcd4-04521ef510c5" />
</p>

#### Example
```
age = 16

if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible to vote")
```
### 6.3 elif Statement
Used when you have multiple conditions to check.

#### Syntax
<p align="center">
<img width="623" height="254" alt="image" src="https://github.com/user-attachments/assets/5f613ec7-debe-4512-abaf-6af45aeee885" />
</p>

#### Example

```
marks = 85

if marks >= 90:
    print("Grade A")
elif marks >= 75:
    print("Grade B")
elif marks >= 60:
    print("Grade C")
else:
    print("Fail")
```
### 6.4 Nested `if`

A `nested if` statement means an if statement **inside another** if statement.

It allows you to check multiple conditions one inside another — useful for complex decision-making.

#### Syntax
<p align="center">
<img width="654" height="251" alt="image" src="https://github.com/user-attachments/assets/2d2cc0a9-b243-41d0-b01a-ef26bfc6c508" />
</p>

#### Example
```
age = 20
citizen = True

if citizen:
    if age >= 18:
        print("You are eligible to vote.")
    else:
        print("You must be 18 or older to vote.")
else:
    print("You must be a citizen to vote.")
```
### 6.5 Indentation is Important
```
if True:
print("Hello")   # ❌ Error — no indentation

if True:
    print("Hello")  # ✅ Correct
```
### 6.6 Summary

| **Type**           | **Description**                    | **Example**              |
| ------------------ | ---------------------------------- | ------------------------ |
| `if`               | Executes code if condition is true | `if x > 0:`              |
| `if...else`        | Either one block executes          | `if x>0: else:`          |
| `if...elif...else` | Multiple conditions                | `if x>0 elif x==0 else:` |
| Nested `if`        | One `if` inside another            | `if x>0: if x%2==0:`     |

### Python Programming Practice Report
```
1.Print your name, age, and favorite hobby in a single line.

2.Display a welcome message: Welcome to Python Learning, <your name>!

3.Print a short poem or quote using multiple `print`() lines.

4.Print a shopping list with each item on a new line.

5.Print your favorite movie name in uppercase letters.
```





