# Day 2 Notes

#Day2 of #100DaysOfLearningAI

---

## Context

Today was about **progress, not perfection**. I focused on understanding **Functions and Lists** in Python.  
These two concepts are extremely important because they help organize code and store multiple values.

Even though it felt confusing at times, I kept practicing small examples until things made sense.

---

## What I Learned Today

---

## 1. Functions (Reusable Code)

A function is a block of code that performs a specific task.  
Instead of writing the same code again and again, we create a function and reuse it.

### Why functions are important:
- Makes code clean and organized
- Avoids repetition
- Easy to debug
- Easy to reuse

### Example:

```python
def greet(name):
    print(f"Hello, {name}!")
```

Calling the function:

```python
greet("Healy")
```

Output:
```
Hello, Healy!
```

---

## Function with Return Value

```python
def add(a, b):
    return a + b
```

Using the function:

```python
result = add(3, 5)
print(result)
```

Output:
```
8
```

---

## 2. Lists (Storing Multiple Values)

Lists allow us to store **multiple values** in a single variable.

### Example:

```python
fruits = ["apple", "banana", "cherry"]
```

Accessing list items:

```python
print(fruits[0])   # apple
print(fruits[1])   # banana
print(fruits[-1])  # cherry (last item)
```

---

## List Operations

```python
fruits.append("orange")   # Add item
fruits.remove("banana")  # Remove item
print(len(fruits))       # Length of list
```

---

## Mini Project 1: Tip Calculator (Angela Yu Inspired)

### Objective:
Practice:
- Variables
- Input
- Type conversion
- Math operations
- Printing output

---

### Code:

```python
bill = float(input("Enter total bill: $"))
tip = int(input("Enter tip percentage: "))
people = int(input("How many people: "))

tip_amount = bill * tip / 100
total_bill = bill + tip_amount
each_person = total_bill / people

print(f"Each person should pay: ${each_person:.2f}")
```

---

### What I Learned:
- `float()` converts text into decimal numbers
- `int()` converts text into whole numbers
- Mathematical operations
- Formatting output using `:.2f`

---

## Mini Project 2: Simple Password Generator

### Objective:
Practice:
- Lists
- Loops
- Random module

---

### Code:

```python
import random

letters = ["a", "b", "c", "d"]
numbers = ["1", "2", "3"]
symbols = ["!", "@", "#"]

password = []

for i in range(3):
    password.append(random.choice(letters))

for i in range(2):
    password.append(random.choice(numbers))

for i in range(2):
    password.append(random.choice(symbols))

random.shuffle(password)

final_password = "".join(password)
print("Generated password:", final_password)
```

---

### What I Learned:
- `random.choice()` picks a random item
- `append()` adds item to list
- `shuffle()` randomizes order
- `join()` converts list to string

---

## Debugging & Learning Strategy

Today I learned that:
- Errors are part of learning
- Printing values helps debugging
- Breaking problems into small steps makes coding easier

---

## Beginner Takeaways

- Functions = reusable logic
- Lists = store multiple values
- Projects help understand concepts faster
- Debugging improves understanding
- Consistency matters more than perfection

---

## Next Steps (Day 3)

Tomorrow I will learn:
- Dictionaries
- Tuples
- More mini projects
- More problem solving

---

## Hashtags

#Day2 #100DaysOfAI #Python #AIJourney #BeginnerCoder #Functions #Lists #MiniProjects
