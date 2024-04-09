# ![Python for Javascript Developers - Control Flow - Ranges](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to identify and use ranges in Python.

## Purpose of Ranges

Python **_ranges_** are a _sequence type_ like _lists_ and _tuples_.

The **range** type represents an immutable sequence of numbers and is commonly used for looping a specific number of times in `for` loops.

_Ranges_ have a class (type) of `range`.

## Basic Syntax

Ranges can only be created by invoking the `range()` class:

```python
for num in range(5):
  print(num)
```

Notice that by default, the sequence starts at `0` and goes up to, but does not include the integer passed in.

Ranges can also generate sequences with a **start** and a **step**:

```python
for even in range(2, 10, 2):
  print(even)
```

When not passed in, the _start_ value defaults to `0` and the _step_ defaults to `1`.

Ranges can also be used to create _lists_ and _tuples_:

```python
nums = list(range(10))
print(nums)
#  [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

odds = tuple(range(1, 10, 2))
print(odds)
#  (1, 3, 5, 7, 9)
```

## Negative Step

If the _step_ is a negative integer, the _sequence_ counts down:

```python
for num in range(5, 0, -1):
  print(num)
```
