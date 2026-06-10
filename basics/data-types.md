# Python Data Types

## What are Data Types?

Data types define the kind of value a variable can store. Python automatically determines the data type when a value is assigned.

Example:

```python
name = "Kunal"
age = 25
height = 5.9
```

---

## Checking Data Types

Use the `type()` function to determine the data type of a variable.

```python
name = "Kunal"
age = 25

print(type(name))
print(type(age))
```

Output:

```text
<class 'str'>
<class 'int'>
```

---

# Numeric Data Types

Python supports three main numeric data types.

## 1. Integer (int)

Integers are whole numbers without decimal points.

```python
age = 25
temperature = -5

print(type(age))
```

Output:

```text
<class 'int'>
```

### Examples

```python
a = 10
b = -100
c = 0
```

---

## 2. Float (float)

Floats are numbers containing decimal points.

```python
price = 99.99
height = 5.8

print(type(price))
```

Output:

```text
<class 'float'>
```

### Examples

```python
pi = 3.14159
salary = 45000.50
```

---

## 3. Complex (complex)

Complex numbers contain a real and imaginary part.

```python
number = 2 + 3j

print(type(number))
```

Output:

```text
<class 'complex'>
```

---

# String Data Type (str)

Strings store text data.

```python
name = "Kunal"
city = 'Gurgaon'
```

Check type:

```python
print(type(name))
```

Output:

```text
<class 'str'>
```

### String Operations

Concatenation:

```python
first_name = "Kunal"
last_name = "Yadav"

full_name = first_name + " " + last_name

print(full_name)
```

Output:

```text
Kunal Yadav
```

---

# Boolean Data Type (bool)

Boolean values represent True or False.

```python
is_student = True
is_employed = False

print(type(is_student))
```

Output:

```text
<class 'bool'>
```

### Examples

```python
print(10 > 5)
```

Output:

```text
True
```

---

# Sequence Data Types

## 1. List

Lists are ordered, mutable collections.

```python
fruits = ["Apple", "Banana", "Mango"]

print(type(fruits))
```

Output:

```text
<class 'list'>
```

### Access Elements

```python
print(fruits[0])
```

Output:

```text
Apple
```

---

## 2. Tuple

Tuples are ordered but immutable.

```python
coordinates = (10, 20)

print(type(coordinates))
```

Output:

```text
<class 'tuple'>
```

### Example

```python
student = ("Kunal", 25)
```

---

## 3. Range

Used to generate a sequence of numbers.

```python
numbers = range(5)

print(type(numbers))
```

Output:

```text
<class 'range'>
```

### Example

```python
for num in range(5):
    print(num)
```

Output:

```text
0
1
2
3
4
```

---

# Set Data Types

Sets store unique values.

```python
numbers = {1, 2, 3, 4}

print(type(numbers))
```

Output:

```text
<class 'set'>
```

### Example

```python
numbers = {1, 2, 2, 3}

print(numbers)
```

Output:

```text
{1, 2, 3}
```

Duplicate values are removed automatically.

---

# Dictionary Data Type (dict)

Dictionaries store data in key-value pairs.

```python
student = {
    "name": "Kunal",
    "age": 25
}

print(type(student))
```

Output:

```text
<class 'dict'>
```

### Access Values

```python
print(student["name"])
```

Output:

```text
Kunal
```

---

# None Type

Represents the absence of a value.

```python
data = None

print(type(data))
```

Output:

```text
<class 'NoneType'>
```

---

# Type Conversion

Python allows conversion between data types.

## Integer to Float

```python
age = 25

print(float(age))
```

Output:

```text
25.0
```

---

## Float to Integer

```python
price = 99.99

print(int(price))
```

Output:

```text
99
```

---

## Integer to String

```python
number = 100

print(str(number))
```

Output:

```text
'100'
```

---

## String to Integer

```python
age = "25"

print(int(age))
```

Output:

```text
25
```

---

# Summary Table

| Data Type | Example          |
| --------- | ---------------- |
| int       | 10               |
| float     | 10.5             |
| complex   | 2 + 3j           |
| str       | "Python"         |
| bool      | True             |
| list      | [1, 2, 3]        |
| tuple     | (1, 2, 3)        |
| set       | {1, 2, 3}        |
| dict      | {"name":"Kunal"} |
| NoneType  | None             |

---

# Best Practices

* Use appropriate data types for your data.
* Convert data types only when necessary.
* Use dictionaries for structured information.
* Use lists when data may change.
* Use tuples for fixed values.

---

# Practice Questions

1. Create variables of type int, float, and string.
2. Use `type()` to check their data types.
3. Convert a string `"100"` into an integer.
4. Create a list of your favorite movies.
5. Create a dictionary containing your name, age, and city.
6. Create a set with duplicate values and observe the output.

---

# Mini Exercise

```python
name = "Kunal"
age = 25
height = 5.8
is_student = True

print(type(name))
print(type(age))
print(type(height))
print(type(is_student))
```

Expected Output:

```text
<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>
```
