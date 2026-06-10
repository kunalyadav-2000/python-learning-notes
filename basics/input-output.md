# Python Input and Output

## Introduction

Input and Output (I/O) are fundamental concepts in programming.

* **Input** allows users to provide data to a program.
* **Output** allows programs to display information to users.

Python provides built-in functions for handling input and output.

---

# Output in Python

The `print()` function is used to display output on the screen.

## Basic Output

```python
print("Hello, World!")
```

Output:

```text
Hello, World!
```

---

## Printing Variables

```python
name = "Kunal"
age = 25

print(name)
print(age)
```

Output:

```text
Kunal
25
```

---

## Printing Multiple Values

```python
name = "Kunal"
age = 25

print(name, age)
```

Output:

```text
Kunal 25
```

---

## Using the `sep` Parameter

The `sep` parameter specifies the separator between values.

```python
print("Python", "Java", "C++", sep=" | ")
```

Output:

```text
Python | Java | C++
```

---

## Using the `end` Parameter

The `end` parameter controls what is printed at the end.

```python
print("Hello", end=" ")
print("World")
```

Output:

```text
Hello World
```

---

# Formatted Output

## String Concatenation

```python
name = "Kunal"

print("Hello " + name)
```

Output:

```text
Hello Kunal
```

---

## f-Strings (Recommended)

f-strings provide a clean and readable way to format output.

```python
name = "Kunal"
age = 25

print(f"My name is {name} and I am {age} years old.")
```

Output:

```text
My name is Kunal and I am 25 years old.
```

---

## Using `.format()`

```python
name = "Kunal"
age = 25

print("My name is {} and I am {} years old.".format(name, age))
```

Output:

```text
My name is Kunal and I am 25 years old.
```

---

# Input in Python

The `input()` function is used to take input from the user.

## Basic Input

```python
name = input("Enter your name: ")

print(name)
```

Example:

```text
Enter your name: Kunal
Kunal
```

---

## Input with a Message

```python
city = input("Enter your city: ")

print("City:", city)
```

Example:

```text
Enter your city: Gurgaon
City: Gurgaon
```

---

# Understanding Input Data Type

The `input()` function always returns a string.

Example:

```python
age = input("Enter your age: ")

print(type(age))
```

Output:

```text
<class 'str'>
```

Even if the user enters a number, Python treats it as a string.

---

# Converting Input Data Types

## String to Integer

```python
age = int(input("Enter your age: "))

print(type(age))
```

Output:

```text
<class 'int'>
```

---

## String to Float

```python
salary = float(input("Enter your salary: "))

print(type(salary))
```

Output:

```text
<class 'float'>
```

---

# Taking Multiple Inputs

## Method 1: Separate Inputs

```python
name = input("Enter name: ")
age = int(input("Enter age: "))
```

---

## Method 2: Single Line Input

```python
name, age = input("Enter name and age: ").split()

print(name)
print(age)
```

Example:

```text
Enter name and age: Kunal 25

Kunal
25
```

---

# Performing Calculations with User Input

## Add Two Numbers

```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

sum_result = num1 + num2

print("Sum:", sum_result)
```

Example:

```text
Enter first number: 10
Enter second number: 20

Sum: 30
```

---

## Calculate Area of a Rectangle

```python
length = float(input("Enter length: "))
width = float(input("Enter width: "))

area = length * width

print("Area =", area)
```

Example:

```text
Enter length: 10
Enter width: 5

Area = 50.0
```

---

# Escape Characters

Escape characters are used to format output.

| Escape Character | Description  |
| ---------------- | ------------ |
| \n               | New Line     |
| \t               | Tab Space    |
| \                | Backslash    |
| '                | Single Quote |
| "                | Double Quote |

## Example

```python
print("Python\nProgramming")
```

Output:

```text
Python
Programming
```

---

## Tab Example

```python
print("Name\tAge")
print("Kunal\t25")
```

Output:

```text
Name    Age
Kunal   25
```

---

# Common Input Errors

## Example 1: Invalid Integer

```python
age = int(input("Enter age: "))
```

User Input:

```text
twenty
```

Output:

```text
ValueError
```

---

## Handling Errors with try-except

```python
try:
    age = int(input("Enter age: "))
    print(age)
except ValueError:
    print("Please enter a valid number.")
```

---

# Real-World Examples

## Greeting User

```python
name = input("Enter your name: ")

print(f"Welcome, {name}!")
```

---

## Calculate Simple Interest

```python
principal = float(input("Principal Amount: "))
rate = float(input("Rate of Interest: "))
time = float(input("Time in Years: "))

interest = (principal * rate * time) / 100

print("Simple Interest:", interest)
```

---

## Student Information

```python
name = input("Student Name: ")
roll_no = input("Roll Number: ")

print("Name:", name)
print("Roll No:", roll_no)
```

---

# Best Practices

* Use meaningful prompts in `input()`.
* Convert input data types when necessary.
* Use f-strings for formatted output.
* Validate user input before processing.
* Handle exceptions using `try-except`.

---

# Summary

* `print()` is used to display output.
* `input()` is used to take user input.
* `input()` always returns a string.
* Use `int()`, `float()`, or `str()` for type conversion.
* f-strings provide clean and readable formatting.
* Error handling improves program reliability.

---

# Practice Questions

1. Take a user's name and display a greeting.
2. Take two numbers and print their sum.
3. Take length and width and calculate area.
4. Create a program to calculate simple interest.
5. Use f-strings to display student information.
6. Use `sep` and `end` parameters in `print()`.

---

# Mini Exercise

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))

print(f"Hello {name}!")
print(f"You are {age} years old.")
```

Expected Output:

```text
Enter your name: Kunal
Enter your age: 25

Hello Kunal!
You are 25 years old.
```
