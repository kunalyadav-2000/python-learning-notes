# Python Variables

## What is a Variable?

A variable is a container used to store data in memory. Variables allow us to save values and use them later in our programs.

## Creating Variables

In Python, variables are created when a value is assigned to them.

```python
name = "Kunal"
age = 25
height = 5.9
```

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

## Variable Naming Rules

### Valid Variable Names

```python
name = "Kunal"
user_age = 25
total_marks = 450
student1 = "Rahul"
```

### Invalid Variable Names

```python
1name = "Kunal"      # Cannot start with a number
user-name = "Rahul"  # Hyphen is not allowed
class = "Python"     # Reserved keyword
```

### Naming Conventions

Use descriptive names:

```python
student_name = "Kunal"
monthly_salary = 50000
total_expenses = 12000
```

Avoid:

```python
a = "Kunal"
x = 50000
```

---

## Multiple Variable Assignment

### Assign Multiple Values

```python
name, age, city = "Kunal", 25, "Gurgaon"

print(name)
print(age)
print(city)
```

### Assign Same Value

```python
x = y = z = 100

print(x)
print(y)
print(z)
```

---

## Variable Types

Python automatically determines the data type.

```python
name = "Kunal"      # String
age = 25            # Integer
salary = 45000.50   # Float
is_student = True   # Boolean
```

Check type:

```python
print(type(name))
print(type(age))
```

Output:

```text
<class 'str'>
<class 'int'>
```

---

## Updating Variables

Variables can be changed at any time.

```python
age = 25

print(age)

age = 26

print(age)
```

Output:

```text
25
26
```

---

## Dynamic Typing

Python allows a variable to change its type.

```python
value = 100

print(type(value))

value = "Python"

print(type(value))
```

Output:

```text
<class 'int'>
<class 'str'>
```

---

## User Input with Variables

```python
name = input("Enter your name: ")

print("Hello", name)
```

Example:

```text
Enter your name: Kunal
Hello Kunal
```

---

## Constants

Python does not have true constants, but uppercase names are commonly used.

```python
PI = 3.14159
MAX_USERS = 100
```

By convention, these values should not be changed.

---

## Best Practices

* Use meaningful variable names.
* Follow snake_case naming convention.
* Avoid single-letter variable names.
* Keep variable names concise but descriptive.
* Use uppercase names for constants.

### Good Example

```python
student_name = "Kunal"
total_marks = 450
is_passed = True
```

### Bad Example

```python
a = "Kunal"
b = 450
c = True
```

---

## Summary

* Variables store data values.
* Python creates variables automatically when assigned.
* Variables can store different data types.
* Variable names should be meaningful and follow naming conventions.
* Python is dynamically typed, allowing variable types to change during execution.

## Practice Questions

1. Create a variable named `city` and store your city name.
2. Create variables for your age and favorite number.
3. Print the type of each variable using `type()`.
4. Assign multiple values to variables in a single line.
5. Take user input and store it in a variable.

## Mini Exercise

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))

print("Name:", name)
print("Age:", age)
```

Expected Output:

```text
Enter your name: Kunal
Enter your age: 25

Name: Kunal
Age: 25
```
