# Day 5 Notes  
#Day5 of #100DaysOfLearningAI

---

## Context: Making Progress 🚀

Today marked an important step in my learning journey. I started understanding how Python is used not just for small scripts, but for real-world data handling and AI workflows.

I focused on:
- Modules
- APIs
- Pandas (Introduction)

This is where Python starts to feel powerful.

---

## 1. What Are Modules?

A **module** is a file that contains Python code (functions, variables, classes) that can be reused.

Instead of writing everything from scratch, Python allows us to import ready-made tools.

---

### Why Modules Matter

Modules help us:
✔ Reuse code  
✔ Stay organized  
✔ Save time  
✔ Use powerful built-in features  

---

### Example: Using a Module

```python
import math

print(math.sqrt(16))
print(math.pi)

Importing Specific Functions

from math import sqrt

print(sqrt(25))


2. What Is an API?

An API (Application Programming Interface) allows different programs to communicate with each other.

In simple terms:
An API lets your program talk to another service and get data.

Real-Life Examples of APIs

Weather apps

Payment systems

Google Maps

Chatbots

Social media feeds

Why APIs Matter in AI

AI systems often:
✔ Fetch data from the web
✔ Send predictions to apps
✔ Talk to databases
✔ Integrate with products

Basic API Concept

You:
➡ Send a request
⬅ Receive a response (usually JSON data)

3. Introduction to Pandas

Pandas is a Python library used for data manipulation and analysis.

It helps us:
✔ Load datasets
✔ Clean data
✔ Filter values
✔ Analyze patterns

This is a core tool in AI and data science.

Installing Pandas : pip install pandas

Importing Pandas: import pandas as pd

4. What Is a DataFrame?

A DataFrame is like a table.

It has:

Rows
Columns
Labeled data

Example:
import pandas as pd

data = {
    "Name": ["Healy", "Alex", "Sam"],
    "Age": [17, 22, 25]
}

df = pd.DataFrame(data)
print(df)

5. Basic Pandas Operations
------View Data
df.head()

-------Get Column
df["Name"]

-------Get Row
df.iloc[0]

-------Check Shape
df.shape

6. Why Pandas Is Important for AI

In AI, data is everything.

Before training models, we must:
✔ Clean data
✔ Organize data
✔ Filter data
✔ Explore data

Pandas helps with all of this.

7. How This Connects to Real AI Work

Real AI workflow:

Data → Cleaning → Processing → Training → Prediction

Pandas handles the data stage.

Beginner Takeaways

✔ Modules = reusable tools
✔ APIs = communication bridges
✔ Pandas = data handling powerhouse

These three together unlock real-world applications.

