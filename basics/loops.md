# Python Loops

## What are Loops?

Loops are used to execute a block of code repeatedly.

Instead of writing the same code multiple times, loops allow us to automate repetitive tasks.

Example:

```python
for i in range(5):
    print("Hello")
```

Output:

```text
Hello
Hello
Hello
Hello
Hello
```

---

# Types of Loops in Python

Python provides two main types of loops:

1. `for` Loop
2. `while` Loop

---

# The for Loop

A `for` loop is used to iterate over a sequence such as a list, string, tuple, or range.

## Syntax

```python
for variable in sequence:
    # code block
```

---

## Example: Iterate Through a List

```python
fruits = ["Apple", "Banana", "Mango"]

for fruit in fruits:
    print(fruit)
```

Output:

```text
Apple
Banana
Mango
```

---

## Example: Iterate Through a String

```python
for letter in "Python":
    print(letter)
```

Output:

```text
P
y
t
h
o
n
```

---

# The range() Function

The `range()` function generates a sequence of numbers.

## Example

```python
for i in range(5):
    print(i)
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

## range(start, stop)

```python
for i in range(1, 6):
    print(i)
```

Output:

```text
1
2
3
4
5
```

---

## range(start, stop, step)

```python
for i in range(0, 11, 2):
    print(i)
```

Output:

```text
0
2
4
6
8
10
```

---

# Using else with for Loop

The `else` block executes when the loop completes normally.

```python
for i in range(3):
    print(i)
else:
    print("Loop completed")
```

Output:

```text
0
1
2
Loop completed
```

---

# Nested for Loops

A loop inside another loop is called a nested loop.

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```

Output:

```text
0 0
0 1
1 0
1 1
2 0
2 1
```

---

# The while Loop

A `while` loop executes as long as a condition remains true.

## Syntax

```python
while condition:
    # code block
```

---

## Example

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

Output:

```text
1
2
3
4
5
```

---

# Infinite Loops

Be careful when using `while` loops.

```python
while True:
    print("Hello")
```

This loop never ends unless stopped manually.

---

# Loop Control Statements

Python provides special statements to control loop execution.

## break Statement

The `break` statement immediately exits the loop.

```python
for i in range(10):
    if i == 5:
        break

    print(i)
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

## continue Statement

The `continue` statement skips the current iteration.

```python
for i in range(5):
    if i == 2:
        continue

    print(i)
```

Output:

```text
0
1
3
4
```

---

## pass Statement

The `pass` statement acts as a placeholder.

```python
for i in range(5):
    pass
```

This code does nothing but avoids syntax errors.

---

# Looping Through Lists

```python
numbers = [10, 20, 30, 40]

for number in numbers:
    print(number)
```

Output:

```text
10
20
30
40
```

---

# Looping Through Dictionaries

```python
student = {
    "name": "Kunal",
    "age": 25,
    "city": "Gurgaon"
}

for key, value in student.items():
    print(key, value)
```

Output:

```text
name Kunal
age 25
city Gurgaon
```

---

# Looping Through a Tuple

```python
colors = ("Red", "Green", "Blue")

for color in colors:
    print(color)
```

Output:

```text
Red
Green
Blue
```

---

# Using enumerate()

The `enumerate()` function provides both index and value.

```python
fruits = ["Apple", "Banana", "Mango"]

for index, fruit in enumerate(fruits):
    print(index, fruit)
```

Output:

```text
0 Apple
1 Banana
2 Mango
```

---

# Real-World Examples

## Sum of Numbers

```python
numbers = [10, 20, 30, 40]

total = 0

for number in numbers:
    total += number

print(total)
```

Output:

```text
100
```

---

## Multiplication Table

```python
num = 5

for i in range(1, 11):
    print(f"{num} x {i} = {num * i}")
```

Output:

```text
5 x 1 = 5
5 x 2 = 10
...
5 x 10 = 50
```

---

## Count Characters in a String

```python
text = "Python"

count = 0

for char in text:
    count += 1

print(count)
```

Output:

```text
6
```

---

# Common Mistakes

## Forgetting to Update a while Loop Variable

```python
count = 1

while count <= 5:
    print(count)
```

This creates an infinite loop because `count` never changes.

Correct version:

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

---

# Best Practices

* Use `for` loops when the number of iterations is known.
* Use `while` loops when the stopping condition is uncertain.
* Avoid infinite loops.
* Use meaningful variable names.
* Keep nested loops simple and readable.

---

# Summary

* Loops execute code repeatedly.
* Python provides `for` and `while` loops.
* `range()` generates sequences of numbers.
* `break` exits a loop.
* `continue` skips an iteration.
* `enumerate()` provides indexes while iterating.
* Loops are useful for processing collections and automating repetitive tasks.

---

# Practice Questions

1. Print numbers from 1 to 10 using a `for` loop.
2. Print even numbers between 1 and 20.
3. Find the sum of numbers from 1 to 100.
4. Create a multiplication table for any number.
5. Count the number of vowels in a string.
6. Use a `while` loop to print numbers from 10 to 1.

---

# Mini Exercise

```python
numbers = [5, 10, 15, 20]

total = 0

for number in numbers:
    total += number

print("Total:", total)
```

Expected Output:

```text
Total: 50
```
