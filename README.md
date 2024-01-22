# Python CheatSheet

## Table of Contents

- [Python CheatSheet](#python-cheatsheet)
  - [Table of Contents](#table-of-contents)
    - [Input and Output](#input-and-output)
      - [Input](#input)
      - [Output](#output)
    - [Data Types](#data-types)
      - [Numbers](#numbers)
      - [Strings](#strings)
      - [Booleans](#booleans)
      - [Lists](#lists)
      - [Tuples](#tuples)
      - [Sets](#sets)
      - [Dictionaries](#dictionaries)
    - [Operators](#operators)
      - [Arithmetic Operators](#arithmetic-operators)
      - [Comparison Operators](#comparison-operators)
      - [Bitwise Operators](#bitwise-operators)
      - [Assignment Operators](#assignment-operators)
      - [Logical Operators](#logical-operators)
      - [Identity Operators](#identity-operators)
      - [Membership Operators](#membership-operators)
    - [Control Flow](#control-flow)
      - [If-Else](#if-else)
      - [Ternary-Operator](#ternary-operator)
      - [For Loop](#for-loop)
      - [While Loop](#while-loop)
      - [Break and Continue](#break-and-continue)
      <!-- - [Pass](#pass) -->
    - [Functions](#functions)
      - [Function Definition](#function-definition)
      - [Function Call](#function-call)
      - [Arguments](#arguments)
      - [Return](#return)
      <!-- - [Lambda Functions](#lambda-functions) -->
    - [Classes](#classes)
      - [Class Definition](#class-definition)
      - [Class Instantiation](#class-instantiation)
      - [Class Methods](#class-methods)
      - [Class Inheritance](#class-inheritance)

## Input and Output

#### Input

```python
input("Enter your name: ")
```

#### Output

```python
print("Hello World!") # Hello World!
# Using sep
print("Hello", "World!", sep="#") # Hello#World!
```

## Data Types

#### Numbers

```python
a = 1 # int
a = 1.0 # float
a = 1 + 2j # complex
```

#### Booleans

```python
a = True
a = False
```

#### Strings

```python
a = "Hello World!"
a = 'Hello World!'
a = """Hello World!"""
a = '''Hello World!'''
# Functions and Methods
print(len(a))   # Returns the length of a string
a.lower()       # Converts a string into lower case
print(a.lower()) # hello world!
a.upper()       # Converts a string into upper case
print(a.upper()) # HELLO WORLD!
a.replace("H", "J") # Replaces a substring with another
print(a.replace("H", "J")) # Jello World!
a.split(" ")    # Splits the string at the specified separator, and returns a list
print(a.split(' ')) # ['Hello', 'World']
a = ' '.join(["Hello", "World!"]) # Turns list into string by using separator between list elements
print(a) # Hello World!
```

#### Lists

```python
a = ["apple", "banana", "cherry"]
a = [1, 2, 3]
a = [True, False, True]
a = [1, "Hello World!", True]
# Accessing
a[0] # 1
a[-1] # True
a[1:3] # ["Hello World!", True]
# Functions and Methods
print(len(a))   # Returns the number of items in a list.
a.append(4)     # Adds an element to the end of the list
a.insert(0, 0)  # Adds an element at the specified position
a.remove(1)     # Removes the first occurrence of the specified
a.pop()         # Removes the last item
a.clear()       # Removes all the elements from the list
a.sort()        # Sorts the list
a.reverse()     # Reverses the order of the list
```

#### Tuples

```python
a = ("apple", "banana", "cherry")
a = (1, 2, 3)
a = (True, False, True)
a = (1, "Hello World!", True)
# Functions and Methods
print(len(a))   # Returns the number of items in a tuple.
a.count(1)      # Returns the number of times a specified value occurs in a tuple
a.index(1)      # Returns the index of the first occurrence of the specified value
a.remove(1)     # Removes the first occurrence of the specified
a.clear()       # Removes all the elements from the tuple
```

_Note:_

- In Python tuples are immutable while lists are mutable.
- _mutability of lists_ means we can modify the list after creation in the other hand _immutability of tuples_ means we can't change the tuple after creation

#### Sets

```python
a = {"apple", "banana", "cherry"}
a = {1, 2, 3}
a = {True, False, True}
# Functions and Methods
print(len(a))   # Returns the number of items in a set.
a.add(4)        # Adds an element to the set
a.remove(4)     # Removes the specified element
a.discard(4)    # Removes the specified element
a.pop()         # Removes the last item
a.clear()       # Removes all the elements from the set
```

**_Note:_**

- The elements in a set must be of the same data type.
- Sets are unordered, so the items will appear in a random order.
- Set items are unchangeable, meaning that we cannot change the items after the set has been created.

#### Dictionaries

```python
a = {1: "Mohamed", 2: 36}
a = {True: "Mohamed", False: 36}
a = {"name": "Mohamed", "age": 36}
# Accessing
a["name"] # Mohamed
a.get("name") # Mohamed
# Functions and Methods
print(len(a))            # Returns the number of items in a dictionary.
a["name"] = "Mohamed"    # Changes the value of a specified key
a["address"] = "ALgeria" # Adds a new key-value pair
a.pop("name")            # Removes the element with the specified key
```

## Operators

#### Arithmetic Operators

| Operator | Description    | Example  |
| -------- | -------------- | -------- |
| `+`      | Addition       | `x + y`  |
| `-`      | Subtraction    | `x - y`  |
| `*`      | Multiplication | `x * y`  |
| `/`      | Division       | `x / y`  |
| `%`      | Modulus        | `x % y`  |
| `**`     | Exponentiation | `x ** y` |
| `//`     | Floor division | `x // y` |

```python
# Difference between division and floor division
print(5 / 2) # 2.5
print(5 // 2) # 2
```

#### Comparison operators

| Operator | Description              | Example  |
| -------- | ------------------------ | -------- |
| `==`     | Equal                    | `x == y` |
| `!=`     | Not equal                | `x != y` |
| `>`      | Greater than             | `x > y`  |
| `<`      | Less than                | `x < y`  |
| `>=`     | Greater than or equal to | `x >= y` |
| `<=`     | Less than or equal to    | `x <= y` |

#### Bitwise Operators

| Operator | Description          | Example  |
| -------- | -------------------- | -------- |
| `&`      | AND                  | `x & y`  |
| `\|`     | OR                   | `x \| y` |
| `^`      | XOR                  | `x ^ y`  |
| `~`      | NOT                  | `~x`     |
| `<<`     | Zero fill left shift | `x << y` |
| `>>`     | Signed right shift   | `x >> y` |

```python
# Example
x = 5 # 0b0101 in binary
y = 3 # 0b0011 in binary
print(x & y)  # 1 (0b0001 in binary)
print(x | y)  # 7 (0b0111 in binary)
print(x ^ y)  # 6 (0b0110 in binary)
print(~x)     # -6 (in two's complement form)
# Those Two Are The Most Useful
print(x << 1) # 10 (0b1010 in binary)
print(x >> 1) # 2 (0b0010 in binary)
```

#### Assignment Operators

| Operator | Description                    | Example   |
| -------- | ------------------------------ | --------- |
| `=`      | Assign                         | `x = 5`   |
| `+=`     | Add and assign                 | `x += 5`  |
| `-=`     | Subtract and assign            | `x -= 5`  |
| `*=`     | Multiply and assign            | `x *= 5`  |
| `/=`     | Divide and assign              | `x /= 5`  |
| `%=`     | Modulus and assign             | `x %= 5`  |
| `**=`    | Exponentiation and assign      | `x **= 5` |
| `//=`    | Floor division and assign      | `x //= 5` |
| `&=`     | Bitwise AND and assign         | `x &= 5`  |
| `\|=`    | Bitwise OR and assign          | `x \|= 5` |
| `^=`     | Bitwise XOR and assign         | `x ^= 5`  |
| `>>=`    | Bitwise right shift and assign | `x >>= 5` |
| `<<=`    | Bitwise left shift and assign  | `x <<= 5` |

#### Logical Operators

| Operator | Description                                             | Example                 |
| -------- | ------------------------------------------------------- | ----------------------- |
| `and`    | Returns True if both statements are true                | `x < 5 and  x < 10`     |
| `or`     | Returns True if one of the statements is true           | `x < 5 or x < 4`        |
| `not`    | Reverse the result, returns False if the result is true | `not(x < 5 and x < 10)` |

#### Identity Operators

| Operator | Description                                            | Example      |
| -------- | ------------------------------------------------------ | ------------ |
| `is`     | Returns True if both variables are the same object     | `x is y`     |
| `is not` | Returns True if both variables are not the same object | `x is not y` |

```python
# Example
x = ["apple", "banana"]
z = x
print(x is z) # True
print(x is not z) # False
```

#### Membership Operators

| Operator | Description                                                                      | Example      |
| -------- | -------------------------------------------------------------------------------- | ------------ |
| `in`     | Returns True if a sequence with the specified value is present in the object     | ` x in y`    |
| `not in` | Returns True if a sequence with the specified value is not present in the object | `x not in y` |

```python
# Example
x = ["apple", "banana"]
print("banana" in x) # True
print("banana" not in x) # False
```

## Control Flow

- Conditional execution: If a condition is met then execute statement. Otherwise skip it.
- Looping: Execute statement multiple times.

#### If Statement

```python
if condition:
    # statement 1
elif condition:
    # statement 2
else:
    # statement 3

# Example
a = 5
if a > 5:
    print("Greater than 5")
elif a < 5:
    print("Less than 5")
else:
    print("Equal to 5")

# Equal to 5
```

#### Ternary-Operator

```python
value_if_true if condition else value_if_false
# Example
a = True
num1 = 5
num2 = 1
print("Hello World!") if a else print("Bye World!") # Hello World!
print(num1) if num1 > num2 else print(num2) # 5
```

#### For Loop

```python
for item in iterable:
    # statement

# Example
list = [2, 6, 4, 5]
for i in list:
    print(i)
# 2
# 6
# 4
# 5
```

#### While Loop

```python
while condition:
    # statement

# Example
i = 1
sum = 0
while i < 3:
    sum = i
    i += 1
print(sum) # 3
```

#### Break and Continue

```python
for item in iterable:
    if condition:
        break # Breaks out of the loop
    if condition:
        continue # Skips this iteration of the loop

# Example
list = [2, 6, 4, 5]
for i in list:
    if i == 6:
        break
    print(i)
# 2
# 6
```

<!-- #### Pass

```python
# Example
for item in iterable:
    pass # Does nothing
``` -->

## Functions

- A function is a reusable piece of code that performs a specific task. It can be
  called from anywhere in a program.

#### Function Definition

```python
def function_name(parameters):
    # statement
```

#### Function Call

```python
function_name(arguments)
```

#### Arguments

- These are values passed into functions when they're called. They represent the data used by
  the function to perform its task.

#### Return

- A function can return a value to the caller using the return statement.

```python
def function_name(parameters):
    # statement
    return value

# Example
def add(a, b):
    return a + b
print(add(1, 2)) # 3
```
