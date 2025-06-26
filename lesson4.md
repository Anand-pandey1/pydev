## lesson 4. Dictionaries & Nested Data 📕

>🔑 1. What is a Dictionary?

>>A dictionary stores key-value pairs.
Think of it like a real dictionary: you look up a word (key) and get its meaning (value).
<br><br>

## ✅ Key Features:

Keys must be unique ❌ (no Dublicates in keys)

Changeable ✅

Unordered ✅ (Python 3.7+ maintains order)


```python
# Creating a dictionary
student = {"name": "Alex", "age": 16, "grade": "A"}

# Accessing values
print(student["name"])  # Alex

# Modifying values
student["age"] = 17

# Adding new key-value pair
student["city"] = "New York"

# Removing key-value pair
del student["grade"] #deletes both key and its value

print(student)  # {'name': 'Alex', 'age': 17, 'city': 'New York'}


```

## Explanation
```python
student = {"name":"alex"}
        # "key" : "value" (saperated by comma)
```
>each key has its own value specified by colon(:)

```python
student["age"] = 17 
# its updates/replace the value ofexisting key (age) with a new value given (17)
```

```python
student["city"] = "New York"
# creates a new entry with a new "key" : "value" pair

#and if we print the dictionary
print(student)
# "name": "Alex", "age": 17, "grade": "A", "city":"New York"
```
<br><br><br>
<hr>

## 📚 6. Nested Dictionaries
You can nest dictionaries inside others:
```python
user = {
    "username": "luna",
    "profile": {
        "age": 21,
        "country": "Japan",
        "hobbies": ["drawing", "gaming"]
    }
}

print(user["profile"]["hobbies"][0])


```
## Explanation
```python
user = {
    "username": "luna", "profile" : {   "age": 21, "country": "Japan", "hobbies": ["drawing", "gaming"] }

    # we have created a new key as (profile) but values are inside curly bracket so it acts like a new dictionary
}

print(user["profile"]["hobbies"][0])  # drawing
# specifies to acces ductionary(user)
# then a key called (profile)
# then inside it another key (hobbies) 
# and finally orint its 1st value(0)
```

<br><br><br>
## 🔄 7. Useful Methods
```python
person.keys()       #  prints all the keys of a dictionary
person.values()     #  prints all the values of a dictionary
person.items()      #  prints all the items(keys ,values) of a dictionary
```

## 🧪 Mini Practice
```python
# Simple dictionary
book = {
    "title": "1984",
    "author": "George Orwell",
    "year": 1949
}
book["genre"] = "Dystopian"
book["year"] = 1950

for k, v in book.items():
    print(f"{k}: {v}")

```

## 📌 Assignment 1

Write a Python script that:

1. Creates a dictionary for a student:
```python
student = {
    "name": "Your Name",
    "age": 20,
    "grades": {"math": 85, "science": 92, "english": 78}
}

```
2. Add a "passed": True key.

3. Print each subject with its grade.

4. Calculate the average grade and print it.

## 📌 Assignment 2

Create a dictionary of a student's details (name, class, marks), update marks, and add a new field.
