# Day 6 Notes

# Day 6: Python for AI — Foundation Complete ✅
#Day6 of #100DaysOfLearningAI

Today I completed the **"Python for AI" course by Dave Ebbelaar**.  
This day was all about learning **important Python skills** that every AI beginner should know before building real projects.

---

## 1. Object-Oriented Programming (OOP) — Using Classes

### What is a Class?
- Think of a class like a **blueprint** for building something.  
- Example: a blueprint of a car — you can build many cars from it.  
- In Python, a class is used to **create objects** with their own data and actions.

### What is an Object?
- An object is a **thing made from a class**.  
- Each object can have **attributes** (data, like name or age) and **methods** (things it can do, like greet).

### Example:

```python
# Step 1: Create a class
class Student:
    def __init__(self, name, age):  # __init__ is called when we create a student
        self.name = name  # attribute: name
        self.age = age    # attribute: age

    def greet(self):      # method: action
        print(f"Hello, my name is {self.name} and I am {self.age} years old.")

# Step 2: Make an object (instance of the class)
student1 = Student("Healy", 17)

# Step 3: Use the object's method
student1.greet()

What we learned here:

class Student: defines a blueprint.

__init__ sets up the object automatically.

self.name and self.age are attributes.

greet() is a method that the object can use.

student1 = Student("Healy", 17) creates a new student.

2. Git & GitHub — Saving and Sharing Code
Why Git?

Git tracks all changes you make in your code.

You can go back to previous versions if something breaks.

GitHub lets you share your work online for recruiters or collaborators.

Basic Git Workflow
# 1. Initialize a Git repository
git init

# 2. Add all your files to Git
git add .

# 3. Commit the changes (take a snapshot)
git commit -m "Completed Day 6 notes and practice"

# 4. Push to GitHub (remote repository)
git push origin main

Pro tips for beginners:

Always write a clear commit message. Example: "Added Day6 OOP notes"

Use GitHub to show progress day by day.

Organize each day in its own folder for clarity.

3. Environment Variables — Keeping Secrets Safe
What is it?

Environment variables store private information like API keys or passwords.

Example: If you are using OpenAI API, you don’t want the key in your code.

How to use:import os

# Read secret from environment
API_KEY = os.getenv("MY_API_KEY")
print(API_KEY)  # Will print the value stored in your environment

Why use it:

Keeps keys/passwords safe.

Makes projects professional.

Allows sharing code without exposing secrets.