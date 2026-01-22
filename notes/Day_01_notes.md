# Day 1 Notes

#Day1 of #100DaysOfLearningAI

---

## Context: Consistency > Perfection 🚀
Setup is done. Now the real work starts. Today’s focus was on **Python Control Flow, Loops, and debugging syntax errors**.  

Even small scripts count — moving from "installing" to "building" is a big step for a beginner.  

**LinkedIn Recap:**  
- Focused on **Control Flow** (if/else)  
- Practiced **Loops** (for, while)  
- Fixed syntax errors independently  
- Built small scripts to understand logic  

---

## Python Concepts Learned

### 1. Control Flow (Making Decisions)
Control flow lets the program **decide what to do based on conditions**.

**Example:**
```python
age = int(input("Enter your age: "))

if age >= 18:
    print("You are an adult!")
else:
    print("You are a minor!")
Key Points:

if checks a condition

else runs when if condition is False

Use comparison operators (>=, <=, ==, !=)

2. Loops (Repeating Tasks)
Loops allow repeating tasks multiple times without rewriting code.

For Loop Example:



for i in range(5):
    print(f"This is loop number {i}")
While Loop Example:

count = 0
while count < 5:
    print(f"Count is {count}")
    count += 1
Key Points:

for loops iterate over a sequence or range

while loops run until a condition is False

Incrementing variables is important to avoid infinite loops

Mini Project: 
Project Name: Number Guess Game

Objective: Practice variables, input, control flow, loops, and logic.

import random

# Step 1: Generate random number
secret_number = random.randint(1, 10)

# Step 2: Initialize guess
guess = 0

# Step 3: Loop until correct guess
while guess != secret_number:
    guess = int(input("Guess a number between 1 and 10: "))
    
    if guess < secret_number:
        print("Too low, try again!")
    elif guess > secret_number:
        print("Too high, try again!")
    else:
        print(f"Congratulations! You guessed it: {secret_number}")
Key Learnings:

random.randint() generates a random number

Loops keep program running until condition is met

if-elif-else handles multiple conditions

int() converts user input from string to integer

Step-by-Step Debugging Tips
Print variables after each step to see values:


print("Secret number:", secret_number)
print("Current guess:", guess)
Helps identify errors and understand flow

Beginner Takeaways
Control Flow helps make decisions

Loops allow repetitive tasks efficiently

Small projects reinforce basic logic and Python syntax

Debugging is part of learning — don’t fear syntax errors

