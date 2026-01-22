# Day 0 Notes

#Day0 of #100DaysOfLearningAI

---

## Context: Zero to One 🚀
The hardest part of learning something new is just starting. Today I officially launched my journey into AI/ML. Over the next few months, I’ll be documenting my transition into tech. No filters — just raw progress as I learn to build AI solutions from scratch.

Kicking off with **Day 1: Python Foundations**, inspired by **Dave Ebbelaar’s guide on Python for AI**, to ensure setup is perfect before writing a single line of code.

**Day 0 LinkedIn Post Recap:**
- Environment Setup: Installing VS Code & Python
- The Basics: Variables, Strings, and Data Types
- First Win: Running my first script without errors

---

## Day 0 Learning: Python Environment Setup

### 1. Installing Python
- Installed **Python 3.11** from [python.org](https://www.python.org/downloads/)
- Verified installation:
```bash
python --version
2. Installing VS Code
Downloaded and installed VS Code

Installed Python extension for syntax highlighting and running code

3. Virtual Environment (venv)
What is a virtual environment?
A virtual environment is an isolated Python environment that allows you to manage packages and dependencies for each project separately without interfering with other projects or system Python.

Why we use it:

Prevents version conflicts between projects

Keeps dependencies organized per project

Makes projects portable and reproducible

How to create and activate a virtual environment:



# Create venv folder
python -m venv venv

# Activate on macOS/Linux
source venv/bin/activate

# Activate on Windows
venv\Scripts\activate

# Verify Python is using the venv
which python   # macOS/Linux
where python   # Windows
Python Basics Learned
1. Variables
Variables store data for use in programs:

python
Copy code
name = "Healy"
age = 17
2. Data Types
int, float, str, bool

3. Printing to Console
python

print("Hello, world!")
print(f"My name is {name}, I am {age} years old.")
4. Comments


# Single-line comment
"""
Multi-line comment
"""
User Input
input() reads user input from the console

Always returns a string, even if numbers are entered

Type Conversion
Convert strings to integers using int() for arithmetic operations

Important because "17" + 1 would give an error, but 17 + 1 works

Variables & Arithmetic Operations
Variables store data for later use

Can perform operations like addition (+), subtraction (-), multiplication (*), division (/)

Printing Output
print() displays information in the console

Concatenate strings with + or use f-strings for cleaner formatting

Step-by-Step Debugging / Understanding
Print variables after each step to see their values:

python

print("Name:", name)
print("Age:", age)
print("Next Year Age:", next_year_age)
Beginner Takeaway
Learned input → process → output flow

Understanding each line helps build confidence for bigger programs

Small projects reinforce basic Python syntax and logic

