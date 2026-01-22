# Day 3 Notes

#Day3 of #100DaysOfLearningAI

---

## Context

Today was about learning how to **store structured data** and make smarter decisions in Python.

I focused on:
- Dictionaries
- Nesting data
- Conditional logic (if / else / elif)
- Real-world style problems

These concepts are very important for AI, data, and backend logic.

---

## 1. Dictionaries (Key-Value Data)

A dictionary stores data in **key : value** format.

### Example:

```python
student = {
    "name": "Healy",
    "age": 17,
    "course": "AI"
}
```

Accessing values:

```python
print(student["name"])
print(student["age"])
```

---

## Modifying Dictionary

```python
student["age"] = 18          # Update
student["city"] = "Toronto" # Add new key
```

---

## Looping Through Dictionary

```python
for key in student:
    print(key, ":", student[key])
```

---

## 2. Nesting (Data Inside Data)

### Dictionary inside dictionary:

```python
students = {
    "student1": {"name": "A", "age": 20},
    "student2": {"name": "B", "age": 22}
}
```

Access:

```python
print(students["student1"]["name"])
```

---

### List inside dictionary:

```python
person = {
    "name": "Healy",
    "skills": ["Python", "AI", "ML"]
}
```

---

## 3. Conditional Logic (Decision Making)

### if statement

```python
age = 18

if age >= 18:
    print("You can vote")
```

---

### if-else

```python
age = 15

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

---

### elif (multiple conditions)

```python
score = 85

if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("Fail")
```

---

## Comparison Operators

| Operator | Meaning |
|---------|--------|
| ==      | Equal |
| !=      | Not equal |
| >       | Greater |
| <       | Less |
| >=      | Greater or equal |
| <=      | Less or equal |

---

## Logical Operators

```python
and
or
not
```

Example:

```python
age = 20
has_id = True

if age >= 18 and has_id:
    print("Entry allowed")
```

---

## Mini Project 1: Simple Grading System

### Objective:
Practice:
- if / elif / else
- user input
- conditions

---

### Code:

```python
marks = int(input("Enter your marks: "))

if marks >= 90:
    print("Grade A")
elif marks >= 80:
    print("Grade B")
elif marks >= 70:
    print("Grade C")
else:
    print("Fail")
```

---

## Mini Project 2: Student Data Manager

### Objective:
Practice:
- Dictionary
- Input
- Storing data

---

### Code:

```python
student = {}

student["name"] = input("Enter name: ")
student["age"] = input("Enter age: ")
student["course"] = input("Enter course: ")

print("\nStudent Info:")
for key in student:
    print(key, ":", student[key])
```

---

## Debugging Learnings

Today I learned:
- KeyError happens if key doesn’t exist
- Indentation matters
- Conditions must be correct

---

## Beginner Takeaways

- Dictionaries store structured data
- Conditions control logic
- Nesting makes complex data possible
- These concepts are used everywhere in AI & backend

---

## Tomorrow (Day 4)

I will learn:
- Loops (deep)
- While loops
- For loops
- Range
- Mini games

---

## Hashtags

#Day3 #100DaysOfLearningAI #Python #Dictionaries #IfElse #AIJourney #Beginner


