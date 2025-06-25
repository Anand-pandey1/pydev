## lesson 3.  Lists, Tuples & Sets
>These are fundamental data structures in Python.
>>These are container types used to store multiple values in a single variable. Each has different properties.
<br><br>

## 📋 1. Lists – Ordered, Mutable
>A list is a collection of items that can be changed (mutable).

✅ Key Features:

Ordered ✅

Changeable ✅

Allows Duplicates ✅ can have same items example ["cherry","cherry"]

```python
# Creating a list
fruits = ["apple", "banana", "cherry"]

# Accessing elements
print(fruits[0])  # apple
print(fruits[2])  # cherry

# Modifying elements
fruits[1] = "mango"     # ['apple', 'mango','cherry']

# Adding elements
fruits.append("orange")      # Adds to the end
print(fruits)                # ['apple', 'mango', 'cherry', 'orange']

fruits.insert(1, "Kiwi")    # Inserts at index 1
print(fruits)               # ['apple', 'kiwi', 'banana', 'cherry', 'orange']

# Removing elements
fruits.remove("cherry")    # Removes a specific item
print(fruits)     # ['apple', 'mango', 'banana','orange']
fruits.pop()      # Removes the last item

print(fruits)     # ['apple', 'kiwi', 'mango']

print("apple" in fruits)    # Membership check → True

```

## 📌 2. Tuples – Ordered, Immutable
>A tuple is like a list, but cannot be changed (immutable).

✅ Key Features:

Ordered ✅

Cannot be changed ❌

Allows Duplicates ✅

```python
# Creating a tuple
numbers = (1, 2, 3, 4)

# Accessing elements
print(numbers[0])  # 1



# Tuples cannot be modified (immutable)
# numbers[1] = 5  ❌ This will cause an error

#⚡🔥
# Converting tuple to list (if modification is needed)
numbers_list = list(numbers)
numbers_list.append(5)
numbers = tuple(numbers_list)

print(numbers)  # (1, 2, 3, 4, 5)
```
explanation
```python
numbers_list = list(numbers)    #creating a new list as number_list and giving the values of ("numbers" a tupple) as List
numbers_list.append(5)          # adding 5 to the list (adds to the end)
numbers = tuple(numbers_list)   # now declaring numbers as tupple to its original form
```

## 🔁 3. Sets – Unordered, Unique Items
>A set is an unordered collection with only unique values.
```python
# Creating a set
numbers = {1, 2, 3, 4, 4, 5}

# Adding elements
numbers.add(6)

# Removing elements
numbers.remove(2)

```
>><b>Set operations (union(|), intersection(&), difference(-))
</b>
```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1 | set2)  # Union {1, 2, 3, 4, 5}
print(set1 & set2)  # Intersection {3}
print(set1 - set2)  # Difference {1, 2}
```

>>Sets ignore duplicates:
```python
nums = {1, 2, 2, 3}
print(nums)  # {1, 2, 3}

```
>>some more on sets
```python
colors = {"red", "green", "blue"}
print("red" in colors)   # True

```

## 🔀 4. Choosing Between Them
--------------------------------------
| Type  | Ordered | Mutable | Duplicates | Use When...                          |
| ----- | ------- | ------- | ---------- | ------------------------------------ |
| List  | ✅       | ✅       | ✅          | You need order and changes           |
| Tuple | ✅       | ❌       | ✅          | Fixed data that shouldn't change     |
| Set   | ❌       | ✅       | ❌          | Fast lookup and no duplicates needed |
<br><br><br>
## 🧪 Mini Practice
```python
# List
animals = ["cat", "dog", "fish"]
animals.append("bird")
print(animals)

# Tuple
point = (4, 5)
x, y = point
print(f"X: {x}, Y: {y}")

# Set
unique_numbers = {1, 2, 3, 2, 1}
print(unique_numbers)
unique_numbers.add(4)

```
<br><br><br>

## 📌 Assignment (Optional)
Write a script that:

Creates a list of 5 favorite movies

Adds one more movie

Removes one you changed your mind about

Prints them all, one per line

Then:

Create a tuple of 3 coordinates (x, y, z)

Create a set of your favorite colors and show how duplicates are removed

Create a set of 5 colors, add a new color, remove one, and perform a union with another set.
