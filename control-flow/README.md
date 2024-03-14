# ![Python Control Flow - Control Flow](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to write logic to implement control flow in Python.

## Control Flow

### Indentation!

Before we start looking at control flow, it’s important to realize that **Python uses indentation to define blocks of code** - not curly braces.

It has always been recommended to use indentation in languages for readability purposes, however, in Python, proper indentation is mandatory!

### Branching with the `if` Statement

Just like in JavaScript, we have the ability to run one of several code paths depending upon the result of conditional expression(s).

Single path `if` statement:

```python
floor = "sticky"
walls = "clean"
if floor == "sticky":   # don't forget the colon
  print("Clean the floor! It's sticky!")
  # more lines of code in this code
  # block need to be indented as well
if walls == "sticky":
  print("Clean the walls! They're sticky!")
```

No parentheses are required around the conditional expression.

Dual path `if..else` statement:

```python
if condition:
  # do something
else:
  # do something else
  # do something else
```

Multi-path `if..elif..else` statement:

```python
if condition1:
  # do something
  # do something
elif condition2:
  # do something else
  # do something else
  # do something else
elif condition3 and condition4:
  # do another thing entirely
  # do another thing entirely
else:
  # else do this stuff
```

The `elif` is not a typo :)

Also note that `else` is always optional.


** 🧠 There is no switch construct in Python **


### You Do (5 minutes) 💪

In your **`app.py`** file, add the following code that accepts text input from the user:

```python
color = input('Enter "green", "yellow", "red": ').lower()
print(f'The user entered {color}')
```

Below that code, write an `if...elif...else` statement that prints out one of the following messages:

- If `green` is entered, print the message `Go!`
- If `yellow` is entered, print the message `Slow Down!`
- If `red` is entered, print the message `Stop!`
- If anything else is entered, print the message `Bogus!`

To run the code, open a terminal in VS Code, then run this command to execute your program: 

```python
python3 app.py
```
