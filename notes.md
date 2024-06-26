# Python Overview

## Developed By
* Python was developed by Guido van Rossum.
* It is used by over 51 million developers.
* Runs on more than a billion devices.
* Generated an income of $743 (8757446.83 IRR).

## Getting Started

1. [Official Python Website](https://www.python.org/)
2. Use online compilers

## Inside Python

### Indentation
* Indentation is important in Python. Proper spaces must be given; otherwise, the whole program may collapse.

### Colon (:)
* Used in function definitions, loops, and conditional statements.

### Function Contents
* Primitives: Numbers, strings, Booleans
* Collections: Lists, dictionaries, sets
* Control Statements: if, elif, loops, etc.
* Range, input/output, tuples
* Interpreter, source code, compiler, bytecode, virtual machine

## Numbers
### Note:
* `print()` is a keyword used for displaying something.

### Types of Numbers in Python:
* **Integers**: 1, 2, 3, 45
* **Floats**: 12.0, .56, 95.0, 10.50
* **Complex**: 5+2j

### Examples:
* Integer: `print(10)` → Output: 10
* Float: `print(10.50)` → Output: 10.50
* Complex: `print(5+2j)` → Output: 5+2j

### Comments
* Comments are used to explain code and are written using the `#` symbol.

### Arithmetic Operations
* **Addition**: `print(5 + 3)` → Output: 8
* **Subtraction**: `print(5 - 3)` → Output: 2
* **Multiplication**: `print(5 * 3)` → Output: 15
* **Division**: `print(5 / 3)` → Output: 1.6667
* **Integer Division**: `print(5 // 3)` → Output: 1
* **Power**: `print(5 ** 3)` → Output: 125
* **Remainder**: `print(5 % 3)` → Output: 2

## Variables
* A variable is a container that stores data values.
* Example:
  ```python
  var = 500
  print(var)  # Output: 500
  ```

### Note:
* Variable names should not start with a number or contain special characters.

### Multiple Variables:
```python
var_one = 500
var_two = "Name"
print(var_one, var_two)  # Output: 500 Name

var1, var2 = 500, "Name"
print(var1, var2)  # Output: 500 Name
```

## Strings
* Combination of alphabets, numbers, and special characters.
* **Single-line strings** should be given between `""` or `''`.
* **Multi-line strings** should be given between triple double quotes `"""` or triple single quotes `'''`.

### Examples:
```python
word = "hi dude"
word2 = "my age is 24!"
para = '''This is
my paragraph.'''
print(word)   # Output: hi dude
print(word2)  # Output: my age is 24!
print(para)   # Output: This is my paragraph.
```

### String Methods
* **Slicing**: `word = "hello"; print(word[1:3])` → Output: el
* **Length**: `word = "hello"; print(len(word))` → Output: 5
* **Strip**: `word = " hello world "; print(word.strip())` → Output: hello world
* **Upper**: `word = "hi"; print(word.upper())` → Output: HI
* **Lower**: `word = "HI"; print(word.lower())` → Output: hi
* **Replace**: `a = "sam"; print(a.replace('m', 'meer'))` → Output: sameer
* **Split**: `a = "sameer"; print(a.split('a'))` → Output: ['s', 'meer']

## Booleans
* Used to represent True or False values

### Examples:
```python
print(1 > 10)  # Output: False
print(1 == 1)  # Output: True
```

## Operators
### Arithmetic Operators:
* **Addition**: `+`
* **Subtraction**: `-`
* **Multiplication**: `*`
* **Division**: `/`
* **Integer Division**: `//`
* **Power**: `**`
* **Remainder**: `%`

### Comparison Operators:
* **Greater Than**: `>`
* **Lesser Than**: `<`
* **Greater Than or Equal To**: `>=`
* **Lesser Than or Equal To**: `<=`
* **Equal To**: `==`
* **Not Equal To**: `!=`

### Logical Operators:
* **And**: `and`
* **Or**: `or`
* **Not**: `not`

### Assignment Operators:
* **Assign**: `=`
* **Add and Assign**: `+=`
* **Subtract and Assign**: `-=`
* **Multiply and Assign**: `*=`
* **Divide and Assign**: `/=`

### Bitwise Operators:
* **AND**: `&`
* **OR**: `|`
* **XOR**: `^`
* **NOT**: `~`
* **Left Shift**: `<<`
* **Right Shift**: `>>`

## Casting
* Casting is used to convert data types.
```python
a = 10
b = 10.10
c = int(b)
print(a, b, c)  # Output: 10 10.1 10
print(type(a), type(b), type(c))  # Output: <class 'int'> <class 'float'> <class 'int'>
```

## Lists
* Lists are collections which are ordered and changeable. Allows duplicate members.
```python
fruits = ["apple", "orange", "cherry"]
print(fruits[0])  # Output: apple

fruits[1] = "banana"
print(fruits)  # Output: ['apple', 'banana', 'cherry']

numbers = [3, 1, 20, 2]
numbers.sort()
print(numbers)  # Output: [1, 2, 3, 20]

numbers.sort(reverse=True)
print(numbers)  # Output: [20, 3, 2, 1]

fruits.append("mango")
print(fruits)  # Output: ['apple', 'banana', 'cherry', 'mango']
```

## Tuples
* Tuples are collections which are ordered and unchangeable. Allows duplicate members.
```python
fruits = ("apple", "banana", "cherry")
print(fruits)  # Output: ('apple', 'banana', 'cherry')
```

## Sets
* Sets are collections which are unordered, unchangeable, and do not allow duplicate members.
```python
fruits = {"apple", "banana", "cherry"}
print(fruits)  # Output: {'banana', 'cherry', 'apple'}
```

## Dictionaries
* Dictionaries are collections which are unordered, changeable, and indexed. No duplicate members.
```python
my_data = {
  "name": "Sameer",
  "age": 16
}
print(my_data.get("name"))  # Output: Sameer
```

## IF, ELIF, ELSE Conditions
### IF Statements:
```python
age = 20
if age > 18:
    print("You can vote")  # Output: You can vote
```

### IF-ELSE Statements:
```python
age = 15
if age > 18:
    print("You can vote")
else:
    print("You are not eligible to vote")  # Output: You are not eligible to vote
```

### ELIF Statements:
```python
age = 18
if age > 18:
    print("You can vote")
elif age == 18:
    print("Happy for your voter ID")  # Output: Happy for your voter ID
else:
    print("You are not eligible to vote")
```

## Functions
* Functions reduce the repetition of code and are defined using the `def` keyword.
```python
def addition(a, b):
    return a + b

print(addition(10, 5))  # Output: 15
```

### Function Examples:
```python
def greet(name):
    return "Hi " + name

print(greet("Sameer"))  # Output: Hi Sameer

def multiply(a, b):
    return a * b

print(multiply(10, 5))  # Output: 50
```

### Return Keyword:
```python
def my_function(a):
    return a * 10

print(my_function(50))  # Output: 500
```
