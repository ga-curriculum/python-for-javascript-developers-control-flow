# ![Python for JavaScript Developers - Control Flow - If...Else](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to use `if...else` statements to implement control flow in Python.

## Indentation

Before we practice more control flow, it’s important to realize that **Python uses indentation to define blocks of code** - not curly braces.

It has always been recommended to use indentation in languages for readability purposes, however, in Python, proper indentation is mandatory!

## Branching with the `if` Statement

Just like in JavaScript, we have the ability to run one of several code paths depending upon the result of conditional expression(s).

Single path `if` statement:

```python
floor = "sticky"
walls = "clean"

 # The colon ':' here signifies the start of the 'if' block.
if floor == "sticky":
    print("Clean the floor! It's sticky!")
    # This is where you would add more lines of code related to the condition
    # They must be indented to be part of the 'if' block.

if walls == "sticky":
    print("Clean the walls! They're sticky!")
```

> Note: Python uses indentation to define blocks of code. This is different from some other
> languages that use curly braces ({ }). The indentation level (usually a tab or four spaces)
> indicates which statements are controlled by the 'if' condition.

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

The `elif` is not a typo! this is pythons clever syntax for `Else If`

Also note that `else` is always optional.

> Note: There is no switch construct in Python

## 🎓 You Do

In your **`control_flow_demo.py`** file, add the following code that accepts text input from the user:

```python
color = input('Enter "green", "yellow", "red": ').lower()
print(f'The user entered {color}')
```

Below that code, write an `if...elif...else` statement that prints out one of the following messages:

- If `green` is entered, print the message `Go!`
- If `yellow` is entered, print the message `Slow Down!`
- If `red` is entered, print the message `Stop!`
- If anything else is entered, print the message `Bogus!`

Use the following command to run this code in your terminal:

```python
python3 control_flow_demo.py
```
