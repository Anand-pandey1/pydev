## lesson 2. Operators#️⃣

> ## 1. Arithmetic Operators
Used to perform mathematical operations:

| Operator | Description         | Example  | Output |
| :------- | ------------------- | -------- | ------ |
| `+`      | Addition            | `5 + 3`  | `8`    |
| `-`      | Subtraction         | `5 - 3`  | `2`    |
| `*`      | Multiplication      | `5 * 3`  | `15`   |
| `/`      | Division            | `5 / 2`  | `2.5`  |
| `//`     | Floor Division      | `5 // 2` | `2`    |
| `%`      | Modulus (Remainder) | `5 % 2`  | `1`    |
| `**`     | Exponentiation      | `2 ** 3` | `8`    |

<hr width="2px">
<br>

> ## 2. Comparison Operators

Used to compare values (returns True or False):

| Operator | Example  | Output  |
| -------- | -------- | ------- |
| `==`     | `5 == 5` | `True`  |
| `!=`     | `5 != 3` | `True`  |
| `>`      | `5 > 3`  | `True`  |
| `<`      | `5 < 3`  | `False` |
| `>=`     | `5 >= 5` | `True`  |
| `<=`     | `3 <= 5` | `True`  |

<hr>

> ## 3. Logical Operators 🚥
Used to combine conditional statements: and return True or False

| Operator | Example          | Output  |
| -------- | ---------------- | ------- |
| `and`    | `True and False` | `False` |
| `or`     | `True or False`  | `True`  |
| `not`    | `not True`       | `False` |

### More about logical operators
>## a. and (Logical AND)

Returns True if both conditions are True.
Otherwise, it returns False.

example
```python
print(True and True)   # True
print(True and False)  # False
print(False and False) # False
```
real world example
```python
age = 18
has_ID = True
print(age >= 18 and has_ID)  # True (Both conditions are True)
```
here
```python 
age >= 18 
#checks whether the age specified is greater than or equal to 18 and after checking it gets that it is 18 so its True
```

> ##  b. or (Logical OR)

Returns True if at least one condition is True.
Only returns False if both conditions are False.

Example:
```python
print(True or False)   # True
print(False or False)  # False
print(True or True)    # True

```
Real world example
```python
Today_is_raining = False
I_have_umbrella = True
print(Today_is_raining or I_have_umbrella)  # True (At least one condition is True)

```
>## c. not (Logical NOT)

Reverses the boolean value:

<u>not</u> True → False

<u>not</u> False → True

Example:
```python
print(not True)  # False
print(not False) # True

```
Real world example
```python
is_daytime = True
print(not is_daytime)  # False (because is_daytime negates True)
```


<br><br><br><br><br><br><br>

## ✅ Task 1:
Create two integer variables a and b.

Perform all arithmetic operations on them and print the results.

Use comparison operators to compare them and print the results.

Create two boolean variables and test them using logical operators.
```python
#task1 example code

a = 10
b = 3

# Arithmetic
print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)

# Comparison
print(a == b)
print(a != b)
print(a > b)
print(a < b)
print(a >= b)
print(a <= b)

# Logical
x = True
y = False
print(x and y)
print(x or y)
print(not x)
```
