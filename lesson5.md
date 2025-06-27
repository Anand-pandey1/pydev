## lesson 5. Conditionals: if, elif, else
> Conditional statements allow your program to make decisions based on conditions.
<br><br>

## comparision operators 
| Operator | Meaning               |
| -------- | --------------------- |
| `==`     | equals                |
| `!=`     | not equals            |
| `>`      | greater than          |
| `<`      | less than             |
| `>=`     | greater than or equal |
| `<=`     | less than or equal    |
<hr>
<br>

## ✅ 1️⃣ Basic if statement
```python
age = 18
if age >= 18:
    print("You are eligible to vote.")
```
>## ✅ Explanation:

>If age >= 18, it prints "You are eligible to vote."
>If the condition is False, nothing happens.

<br>
<br>
<hr>
<br>

## ✅ 2️⃣ if + else
```python
age = 16
if age >= 18:
    print("You are eligible to vote.")
else:
    print("You are not eligible to vote.")
```
> ## ✅ Explanation:

>If age >= 18, the first block runs.
>Otherwise, the else block runs.

<br>
<br>
<hr>
<br>

## ✅ 3️⃣ if + elif + else
```python
marks = 75

if marks >= 90:
    print("Grade: A")
elif marks >= 75:
    print("Grade: B")
elif marks >= 60:
    print("Grade: C")
else:
    print("Grade: F")
```
>## ✅ Explanation:

>If marks >= 90, it prints "Grade: A".

>If marks >= 75 but < 90, it prints "Grade: B".

>If marks >= 60 but < 75, it prints "Grade: C".

>If none of these are True, it prints "Grade: F".

<br><br><hr><br>

## ✅ 4. Nested if Statements
>An if statement inside another if.
```python
age = 20
citizen = True

if age >= 18:
    if citizen:
        print("You can vote.")
    else:
        print("You need to be a citizen to vote.")
else:
    print("You are too young to vote.")

```
>## ✅ Explanation:

The first if checks if age >= 18.

The second if checks if the person is a citizen.

<br><br><br>

## ✅ 5️⃣ if, else with Logical operators
```python
age = 25
has_id = True

if age >= 18 and has_id:
    print("Entry allowed")
else:
    print("Entry denied")

```
<br><hr><br><br>

## 🧪 Mini Practice
```python
temperature = 30

if temperature > 35:
    print("It's really hot!")
elif temperature > 25:
    print("It's warm.")
else:
    print("It's cool.")

```

## 📌 Assignment (Optional)
Write a program that:

1️⃣ Asks for a user’s age (you can hardcode the value).

2️⃣ If under 13: print “Child”

3️⃣ If 13–17: print “Teenager”

4️⃣ If 18+: print “Adult”

Then add:

>A variable has_ticket = True/False

>If age >= 18 and has_ticket == True, print “Welcome to the movie!”

