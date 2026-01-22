# Day 11: AWS AI Practitioner Preparation & Python Data Practice
#Day11 of #100DaysOfLearningAI

---

## 1. Context & Goal

Today’s goal was twofold:

1. **AWS Certified AI Practitioner (AIF-C01) Prep**
   - Revising core AI concepts
   - Understanding how AWS AI services are applied in real-world scenarios

2. **Python Practice for Data Handling**
   - Working with **NumPy** and **Pandas**
   - Exploring arrays, DataFrames, and basic data analysis
   - Connecting Python skills to AI workflows

> Consistency is more important than perfection. Every small step helps build strong foundations.

---

## 2. AWS AI Practitioner Key Concepts

### Artificial Intelligence (AI)
- AI is the simulation of human intelligence in machines.
- **Example:** Chatbots, recommendation engines, self-driving cars

### Machine Learning (ML)
- ML is a subset of AI where machines **learn from data** rather than explicit rules.
- **Example:** Email spam detection

### Deep Learning (DL)
- Uses **neural networks with multiple layers** for complex tasks
- **Example:** Image recognition, speech recognition

### Generative AI
- AI that **creates new content** like text, images, or audio.
- **Example:** ChatGPT, DALL·E

---

## 3. AWS AI Services Overview

### Amazon SageMaker
- **Purpose:** Build, train, and deploy ML models at scale
- **Use Case:** Predicting customer churn or sales forecasting

### Amazon Rekognition
- **Purpose:** Image & video analysis
- **Use Case:** Facial recognition, object detection

### Amazon Comprehend
- **Purpose:** Natural Language Processing (NLP)
- **Use Case:** Sentiment analysis, extracting key phrases

### Amazon Lex
- **Purpose:** Build chatbots and conversational AI
- **Use Case:** Customer support bot

> **Tip for Beginners:** Always try to **connect these services to mini-projects**. For example, use a CSV dataset with SageMaker or a small text with Comprehend.

---

## 4. Python Practice: NumPy & Pandas

Python is the bridge between your AI theory and practical implementation. Today, we practiced handling and exploring data.

---

### 4.1 NumPy – Numerical Python

NumPy helps handle arrays and perform numerical operations efficiently.

```python
import numpy as np

# Create a simple array
arr = np.array([1, 2, 3, 4, 5])

# Sum of elements
print("Sum of array:", np.sum(arr))

# Mean of elements
print("Mean of array:", np.mean(arr))

# Perform arithmetic operations
arr2 = arr * 2
print("Array multiplied by 2:", arr2)

Key Concepts:

Arrays: Store multiple numbers in a single structure

Vectorized operations: Perform calculations on entire arrays at once

NumPy is faster than standard Python lists for numerical tasks

4.2 Pandas – Data Analysis

Pandas is essential for working with structured data using DataFrames.

import pandas as pd

# Create a DataFrame
data = {'Name': ['Alice', 'Bob', 'Charlie'],
        'Age': [25, 30, 35],
        'Department': ['AI', 'ML', 'Data Science']}
df = pd.DataFrame(data)

# View first rows
print(df.head())

# Describe numerical data
print(df.describe())

# Access a column
print(df['Age'])

# Filter rows
print(df[df['Age'] > 28])


Key Concepts:

DataFrame: Like a spreadsheet in Python

Series: A single column in DataFrame

Data exploration: head(), describe(), filtering, selecting columns

5. Connecting Python & AWS AI

Python Skills → AWS AI Practical Use

Arrays → Prepare numeric features for ML models

DataFrames → Clean and analyze datasets for SageMaker

Text analysis in Pandas → Feed into Comprehend for NLP tasks

Example: Take a small CSV dataset, clean it with Pandas, convert numeric columns to NumPy arrays, then use it in SageMaker to train a simple ML model.

6. Beginner-Friendly Takeaways

AWS AI services make theory practical

Don’t just memorize — try to relate to mini-projects

Python is your toolkit

NumPy & Pandas are fundamental for ML workflows

Daily practice reinforces learning

Small exercises each day help retain concepts

Document everything

Update GitHub repo with notes and mini-projects

# --------------------------
# Day 11 Mini-Projects: NumPy & Pandas
# --------------------------

# 1️⃣ NumPy Practice
import numpy as np

# Create arrays
arr = np.array([10, 20, 30, 40, 50])
print("Array:", arr)

# Compute sum, mean, min, max
print("Sum:", np.sum(arr))          # Sum: 150
print("Mean:", np.mean(arr))        # Mean: 30.0
print("Min:", np.min(arr))          # Min: 10
print("Max:", np.max(arr))          # Max: 50

# Multiply arrays by 2
arr_multiplied = arr * 2
print("Array multiplied by 2:", arr_multiplied)
# Output: [20 40 60 80 100]


# 2️⃣ Pandas Practice
import pandas as pd

# Create a DataFrame
data = {
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [25, 30, 35, 28],
    'Department': ['AI', 'ML', 'Data Science', 'AI']
}
df = pd.DataFrame(data)

# View first rows
print("\nDataFrame head():")
print(df.head())

# Describe numerical data
print("\nDataFrame describe():")
print(df.describe())
# Output: count, mean, std, min, max for Age column

# Access a single column
print("\nAges of all employees:")
print(df['Age'])

# Filter rows (Age > 28)
print("\nEmployees older than 28:")
print(df[df['Age'] > 28])
# Output: Bob (30), Charlie (35)


# 3️⃣ Integration Exercise: CSV dataset simulation
# For simplicity, we'll simulate loading a CSV using a dictionary

csv_data = {
    'Feature1': [5, 10, 15, 20, 25],
    'Feature2': [2, 4, 6, 8, 10],
    'Label': [0, 1, 0, 1, 0]
}
df_csv = pd.DataFrame(csv_data)

# Explore the CSV-like data
print("\nCSV Data head():")
print(df_csv.head())

print("\nCSV Data description:")
print(df_csv.describe())

# Convert numeric columns to NumPy arrays
features = df_csv[['Feature1', 'Feature2']].to_numpy()
labels = df_csv['Label'].to_numpy()

print("\nFeatures as NumPy array:")
print(features)
# Output: 2D array [[5 2] [10 4] [15 6] [20 8] [25 10]]

print("\nLabels as NumPy array:")
print(labels)
# Output: [0 1 0 1 0]

# Print statistics manually
print("\nManual stats for Feature1:")
print("Sum:", np.sum(features[:, 0]))
print("Mean:", np.mean(features[:, 0]))
print("Min:", np.min(features[:, 0]))
print("Max:", np.max(features[:, 0]))
