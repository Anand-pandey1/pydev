## 🧠 Lesson 6: Loops — for, while
>Loops allow you to repeat a block of code multiple times.

<br>
<br>

## 🔁 1️⃣ for loops

>Used to iterate (repeat) over a sequence (list, string, range, etc.).
```python
for i in range(5):  # Loops from 0 to 4
    print("Hello", i)
```
## ✅ Explanation:

range(5) generates numbers from 0 to 4 (not including 5).

i takes each value in the range.

The loop prints "Hello" followed by the value of i.

<br>
<hr>

## values of range()
```python
     ##range(start, stop, step) 
for i in range(1, 6, 2):
    print(i)  # 1, 3, 5
```
>>Explanation:
>>range(1,6,2) generates number from 1 - 5 but skips 1 value and steps to another each time

## 👉loop through strings:
```python
for char in "hello":
    print(char)
##prints each character of word hello separately
```


## 👉loop through List Items:
```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
## prints each item of list separately

```


<br>
<br>

## 🔁 2️⃣ while loops

>Repeats code while a condition is True.

```python
count = 0
while count < 5:
    print("Count:", count)
    count += 1  # Increases count by 1
##prints from 0 - 4
```
## ✅ Explanation:

The loop runs while count < 5.

count += 1 increases count by 1 in each iteration.

only prints till count is less than 5 like till 4

## 3. Loop Control Statements
break → Exits the loop.

continue → Skips the current iteration and moves to the next.

```python
for i in range(5):
    if i == 3:
        break  # Stops loop at 3
    print(i)

for i in range(5):
    if i == 2:
        continue  # Skips 2 and then continues
    print(i)

```

<br><br>

## 📌 Assignment

>✅ Write a program that:

>Loops from 1 to 10

>Use a while loop to print numbers from 10 to 1.

>Prints only even numbers

>Stops the loop if it reaches 8

