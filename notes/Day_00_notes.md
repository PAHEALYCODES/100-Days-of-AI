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
Python Basics 

1. Variables
Variables store data for use in programs:

name = "Healy"
age = 17

2. Data Types
int, float, str, bool

3. Printing to Console

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

1. Variables (Data Containers)
Definition: A label for a value you want to use later.

Analogy: A box with a name on it.

Rule: If you change the value, the old one is gone.


age = 25       # Box 'age' holds 25
age = 26       # Box 'age' now holds 26 (25 is deleted)

2. Math Symbols (Arithmetic)
Python works like a calculator, but watch out for the symbols:

+ Add

- Subtract

* Multiply (Use the star, not x)

/ Divide (Use the forward slash)

3. Printing (Showing Output)
How to mix text and variables together.

Option A: The Old Way (Harder) You use + to glue text. Warning: It does not add spaces for you.


print("I am " + name)  # You must add the space inside the quotes manually
Option B: f-Strings (Easier/Recommended) Put an f before the quote and use {} for variables.


print(f"I am {name}")  # Python handles the spacing automatically

4. Debugging (The "Print Check")
If your code breaks, don't guess. Add a print line to check the "invisible" values.

Step 1: input() gets the data.

Step 2: process does the math.

Step 3: print() shows the result.

Beginner Mantra:

Input (Get ingredients) → Process (Cook them) → Output (Serve the meal)

