# Day 7 Notes
# Day 7: Python Practice — Logic & Loops
#Day7 of #100DaysOfLearningAI

Today was all about **putting Python theory into practice** using Angela Yu’s "100 Days of Code" course.  
I focused on **logic and loops** by building **two mini-projects**.  

---

## 1. Tip Calculator

### Objective
- Learn to take user input.
- Practice basic **math operations**.
- Use **formatted strings** for output.

### Key Concepts
- **Input**: Reading user data from the console.
- **Type conversion**: Converting string input to numbers using `int()` or `float()`.
- **Arithmetic operations**: Addition, subtraction, multiplication, division.
- **f-strings**: Formatting output neatly.

### Example Code

```python
# Tip Calculator

print("Welcome to the Tip Calculator!")

# Ask for total bill amount
bill = float(input("What was the total bill? $"))

# Ask for tip percentage
tip_percentage = int(input("What percentage tip would you like to give? 10, 12, or 15? "))

# Ask for number of people to split
people = int(input("How many people to split the bill? "))

# Calculate total tip
tip = bill * tip_percentage / 100

# Total bill including tip
total_bill = bill + tip

# Amount per person
bill_per_person = total_bill / people

# Round to 2 decimal places and print
print(f"Each person should pay: ${bill_per_person:.2f}")

What I learned from this project:

Taking user input and converting types properly.

Using basic math operators to solve real-life problems.

Formatting output with f"" for readability.

Using variables to store and reuse data.
2. Password Generator
Objective

Learn to use loops and lists.

Understand string concatenation and randomization.

Build a simple secure password generator.

Key Concepts

Lists: Store multiple items.

Loops: Repeat actions multiple times.

Random module: Generate random selections.

String manipulation: Combine letters, numbers, and symbols.

Example Code
import random

print("Welcome to the Password Generator!")

# Ask user how many letters, numbers, and symbols
letters = int(input("How many letters would you like in your password? "))
numbers = int(input("How many numbers? "))
symbols = int(input("How many symbols? "))

# Define possible characters
letter_chars = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
number_chars = "0123456789"
symbol_chars = "!@#$%^&*()"

# Create empty password list
password_list = []

# Add random letters
for _ in range(letters):
    password_list.append(random.choice(letter_chars))

# Add random numbers
for _ in range(numbers):
    password_list.append(random.choice(number_chars))

# Add random symbols
for _ in range(symbols):
    password_list.append(random.choice(symbol_chars))

# Shuffle the list for randomness
random.shuffle(password_list)

# Convert list to string
password = "".join(password_list)

print(f"Your password is: {password}")


What I learned from this project:

How to use loops to repeat tasks.

Working with lists and random selection.

Building practical Python scripts that solve problems.

Understanding the importance of shuffling for randomness.

