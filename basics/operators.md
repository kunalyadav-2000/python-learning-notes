# Python Operators

## What are Operators?

Operators are special symbols used to perform operations on variables and values.

Example:

```python
a = 10
b = 5

print(a + b)
```

Output:

```text
15
```

In this example, `+` is an operator.

---

# Types of Operators in Python

Python provides several types of operators:

1. Arithmetic Operators
2. Assignment Operators
3. Comparison Operators
4. Logical Operators
5. Identity Operators
6. Membership Operators
7. Bitwise Operators

---

# 1. Arithmetic Operators

Arithmetic operators are used for mathematical calculations.

| Operator | Description    | Example |
| -------- | -------------- | ------- |
| +        | Addition       | 10 + 5  |
| -        | Subtraction    | 10 - 5  |
| *        | Multiplication | 10 * 5  |
| /        | Division       | 10 / 5  |
| %        | Modulus        | 10 % 3  |
| //       | Floor Division | 10 // 3 |
| **       | Exponentiation | 2 ** 3  |

## Examples

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
print(a // b)
print(a ** b)
```

Output:

```text
13
7
30
3.3333333333333335
1
3
1000
```

---

# 2. Assignment Operators

Assignment operators assign values to variables.

| Operator | Example | Equivalent To |
| -------- | ------- | ------------- |
| =        | x = 5   | x = 5         |
| +=       | x += 3  | x = x + 3     |
| -=       | x -= 3  | x = x - 3     |
| *=       | x *= 3  | x = x * 3     |
| /=       | x /= 3  | x = x / 3     |
| %=       | x %= 3  | x = x % 3     |

## Examples

```python
x = 10

x += 5
print(x)

x -= 3
print(x)

x *= 2
print(x)
```

Output:

```text
15
12
24
```

---

# 3. Comparison Operators

Comparison operators compare two values and return `True` or `False`.

| Operator | Description              |
| -------- | ------------------------ |
| ==       | Equal to                 |
| !=       | Not equal to             |
| >        | Greater than             |
| <        | Less than                |
| >=       | Greater than or equal to |
| <=       | Less than or equal to    |

## Examples

```python
a = 10
b = 5

print(a == b)
print(a != b)
print(a > b)
print(a < b)
```

Output:

```text
False
True
True
False
```

---

# 4. Logical Operators

Logical operators combine multiple conditions.

| Operator | Description                                    |
| -------- | ---------------------------------------------- |
| and      | Returns True if both conditions are True       |
| or       | Returns True if at least one condition is True |
| not      | Reverses the result                            |

## Examples

```python
age = 20
has_id = True

print(age >= 18 and has_id)
print(age < 18 or has_id)
print(not has_id)
```

Output:

```text
True
True
False
```

---

# 5. Identity Operators

Identity operators compare memory locations.

| Operator | Description                               |
| -------- | ----------------------------------------- |
| is       | Returns True if objects are identical     |
| is not   | Returns True if objects are not identical |

## Example

```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)
print(a is c)
```

Output:

```text
True
False
```

Although `a` and `c` contain the same values, they are different objects in memory.

---

# 6. Membership Operators

Membership operators check whether a value exists in a sequence.

| Operator | Description          |
| -------- | -------------------- |
| in       | Value exists         |
| not in   | Value does not exist |

## Example

```python
fruits = ["Apple", "Banana", "Mango"]

print("Apple" in fruits)
print("Orange" in fruits)
```

Output:

```text
True
False
```

---

# 7. Bitwise Operators

Bitwise operators work on binary numbers.

| Operator | Description |
| -------- | ----------- |
| &        | AND         |
| |        | OR          |
| ^        | XOR         |
| ~        | NOT         |
| <<       | Left Shift  |
| >>       | Right Shift |

## Example

```python
a = 5
b = 3

print(a & b)
print(a | b)
```

Output:

```text
1
7
```

Bitwise operators are mainly used in low-level programming and optimization.

---

# Operator Precedence

Python follows a specific order when evaluating expressions.

Example:

```python
result = 10 + 5 * 2

print(result)
```

Output:

```text
20
```

Multiplication happens before addition.

Use parentheses to control evaluation:

```python
result = (10 + 5) * 2

print(result)
```

Output:

```text
30
```

---

# Real-World Examples

## Calculate Total Price

```python
price = 500
quantity = 3

total = price * quantity

print(total)
```

Output:

```text
1500
```

---

## Check Voting Eligibility

```python
age = 20

print(age >= 18)
```

Output:

```text
True
```

---

## Login Validation

```python
username = "admin"
password = "1234"

print(username == "admin" and password == "1234")
```

Output:

```text
True
```

---

# Summary

* Operators perform actions on variables and values.
* Arithmetic operators are used for calculations.
* Comparison operators return Boolean values.
* Logical operators combine conditions.
* Identity operators compare objects.
* Membership operators check presence in collections.
* Assignment operators update variable values.

---

# Practice Questions

1. Find the result of:

```python
10 + 5 * 2
```

2. Check if `25` is greater than `18`.

3. Create a list of fruits and check whether `"Mango"` exists.

4. Use `and` and `or` operators with two conditions.

5. Calculate the square of a number using `**`.

---

# Mini Exercise

```python
num1 = 20
num2 = 4

print("Addition:", num1 + num2)
print("Subtraction:", num1 - num2)
print("Multiplication:", num1 * num2)
print("Division:", num1 / num2)

print("Greater Than:", num1 > num2)
print("Equal To:", num1 == num2)
```

Expected Output:

```text
Addition: 24
Subtraction: 16
Multiplication: 80
Division: 5.0
Greater Than: True
Equal To: False
```
