# ![Python Control Flow - Conditional Expressions](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to implement conditional expressions in the Python language.

# Conditional Expressions in Python

Control flow typically comes down to different code paths executing according to the evaluation of **conditional expressions**.

In other words, if the **conditional expression** evaluates to *truthiness*, do this stuff, optionally, do something else.

Let’s review some of the logic and fundamentals of conditional expressions.

## Boolean Values

Python has two logical boolean values: `True` and `False`.

Most logical operations result in one of these two values. They work exactly the same as in JS but are always written with a starting capital letter in Python.

## Truthy & Falsy in Python

Like JS, every piece of data in Python is considered either **truthy** or **falsy**.

Conditional expressions for `if` statements, etc., rely on an expression evaluating to `True`/**truthy** or `False`/**falsy** to determine which path the code will follow.

Just like in JavaScript, most things in Python are considered to be truthy.

Here’s what is **falsy** in Python:

- `False`
- `None`
- Zero in any numeric type: `0`, `0.0` and `0j`
- Empty sequences or collections:
    - `''` (empty string)
    - `[]` (empty list)
    - `()` (empty tuple)
    - `{}` (empty dictionary)
    - `range(0)` (empty range)

<aside>
⚠️ Note that [] and {} in JavaScript are truthy, not falsy as in Python.

</aside>

## Comparison Operators

Python has all the same comparison operators as JavaScript:

- `<` - less than
- `>` - greater than
- `<=` - less than or equal
- `>=` - greater than or equal
- `==` - equal to
- `!=` - not equal to

Note that in Python, there’s only one equality operator. The `==` in Python is the same as `===` in JavaScript.

### Examples

```python
8 > 8
# => False — 8 is not greater than 8.

8 >= 8
# => True — This checks if 8 is greater than or equal to 8, and they are equal.

8 < 8
# => False — 8 is not less than 8.

7 == 7
# => True — 7 is equal to 7.

7 == "7"
# => False — One is an integer and the other is a string.

7 != 7
# => False — This checks if they aren't equal. Because does 7 equal 7, it's `False`.

6 != 7
# => True — 6 is not equal to 7.

```

## Logical Operators

Luckily, the amazing logical operators we used in JavaScript work the same way in Python except Python uses English words instead of symbols:

- `or` is the same as `||`
- `and` is the same as `&&`

Again, they work just like they did in JS, which means they always return either the **first** or the **second** operand as follows:

### `or`

If the first operand is truthy, return it, otherwise return the second operand.

### `and`

If the first operand is falsy, return it, otherwise return the second operand.

### Examples

```python
True or False
# => True

False or True
# => True

'hello' or 0
# => 'hello'

0 or 'hello'
# => 'hello'

True and False
# => False

False and True
# => False

'hello' and 0
# => 0

0 and 'hello'
# => 0

'hello' and 'tacos'
# => 'tacos'
```
