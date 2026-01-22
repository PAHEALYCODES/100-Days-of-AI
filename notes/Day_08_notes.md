# Day 8: Functions & Caesar Cipher
#Day8 of #100DaysOfLearningAI

Today’s focus: **Unlocking functions in Python**.  
I practiced building a **Caesar Cipher** to encrypt and decrypt text — this helped me understand how to **pass data into functions** and **reuse code efficiently**.

---

## 1. What is a Function?

### Definition
- A function is a **block of code** that performs a specific task.
- Functions help you **organize your code**, **reuse logic**, and **avoid repeating yourself**.

### Why functions are important
1. **Reusable code** — write once, use multiple times.
2. **Easier to debug** — isolate errors inside a function.
3. **Clearer structure** — makes programs readable for you and others.

---

## 2. Caesar Cipher Project

### Objective
- Build a program that can **encrypt** and **decrypt** messages.
- Practice **loops, strings, and functions**.

### How Caesar Cipher works
- Each letter in the message is **shifted by a certain number** in the alphabet.  
- Example: Shift = 3  
  - "A" → "D"  
  - "B" → "E"

---

### Step 1: Define the function

```python
# Caesar Cipher Function
def caesar(text, shift, direction):
    result = ""
    for char in text:
        if char.isalpha():  # Only shift letters
            # Find the alphabet index (0-25)
            ascii_offset = 65 if char.isupper() else 97
            # Shift character and wrap around with modulo 26
            shifted = (ord(char) - ascii_offset + shift) % 26 + ascii_offset
            result += chr(shifted)
        else:
            # Keep non-letters unchanged
            result += char
    if direction == "decode":
        # Reverse shift for decoding
        return caesar(result, -shift, "encode")
    return result
Step 2: Take user input
# User input
direction = input("Type 'encode' to encrypt, type 'decode' to decrypt: ").lower()
text = input("Type your message: ")
shift = int(input("Type the shift number: "))

# Call the function
output = caesar(text, shift, direction)
print(f"The {direction}d text is: {output}")

Key Concepts Learned

Functions:

def caesar(...) defines the function.

Parameters (text, shift, direction) let the function accept different inputs.

return sends the result back to use later.

Loops:

for char in text: iterates over each character in the input message.

Conditional statements:

if char.isalpha() ensures only letters are encrypted.

else keeps spaces, punctuation, and numbers unchanged.

ASCII codes:

ord(char) converts a character to its numeric ASCII code.

chr(number) converts back from number to character.

Modular arithmetic:

(ord(char) - ascii_offset + shift) % 26 + ascii_offset ensures letters wrap around the alphabet.

Reusability:

Functions allow encoding or decoding with one block of code, instead of rewriting logic.