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
      - [Assignment Operators](#assignment-operators)
      - [Comparison Operators](#comparison-operators)
      - [Logical Operators](#logical-operators)
      - [Identity Operators](#identity-operators)
      - [Membership Operators](#membership-operators)
      - [Bitwise Operators](#bitwise-operators)
    - [Control Flow](#control-flow)
      - [If-Else](#if-else)
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
print("Hello World!")
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

_Note:_

- The elements in a set must be of the same data type.
- Sets are unordered, so the items will appear in a random order.
- Set items are unchangeable, meaning that we cannot change the items after the set has been created.

#### Dictionaries

```python
a = {1: "John", 2: 36}
a = {True: "John", False: 36}
a = {"name": "John", "age": 36}
# Accessing
a["name"] # John
a.get("name") # John
# Functions and Methods
print(len(a))   # Returns the number of items in a dictionary.
a["name"] = "Jane" # Changes the value of a specified key
a["address"] = "Doe" # Adds a new key-value pair
a.pop("name")   # Removes the element with the specified key
```
