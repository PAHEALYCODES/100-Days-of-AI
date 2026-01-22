# Day 12 Notes

# Day 12 Notes

#Day12 of #100DaysOfLearningAI

---

## Context: AWS AI + Python Practice 🚀

Today, I focused on connecting **cloud AI services** with **practical Python data handling**.  

Inspired by learning from AWS AI Practitioner concepts, I explored two AWS AI services:

1. **Amazon SageMaker** – a platform to build, train, and deploy machine learning models easily.  
2. **Amazon Rekognition** – a service for image and video analysis like detecting faces, labels, and objects.

Alongside this, I continued **Python practice with NumPy and Pandas** to manipulate datasets — an essential skill for AI workflows.

Every small step is like building a superpower — one line of code, one dataset at a time. ⚡

---

## AWS AI Services Overview

### 1. Amazon SageMaker
- Fully managed ML platform.
- Lets you train models without setting up servers manually.
- Provides pre-built algorithms, Jupyter notebooks, and deployment options.

**Key Concepts for Beginners:**
- **Notebook Instances**: Like a Python workspace in the cloud.
- **Training Jobs**: Where your ML model learns from data.
- **Endpoints**: Where your model is deployed for predictions.

---

### 2. Amazon Rekognition
- AI service for **image and video analysis**.
- Can detect:
  - Faces, emotions, and facial attributes
  - Objects and scenes
  - Text in images
- Very useful for real-world applications like security, retail analytics, or photo tagging.

**Python Integration Example (Boto3):**
```python
import boto3

# Initialize Rekognition client
rekognition = boto3.client('rekognition', region_name='us-east-1')

# Example: Detect labels in an image
image_file = 'example.jpg'
with open(image_file, 'rb') as img:
    response = rekognition.detect_labels(Image={'Bytes': img.read()}, MaxLabels=5)

# Print detected labels
for label in response['Labels']:
    print(label['Name'], ":", label['Confidence'])
Python Practice: NumPy & Pandas
1️⃣ NumPy Exercises
python
Copy code
import numpy as np

# Create an array of numbers
arr = np.array([5, 10, 15, 20, 25])
print("Array:", arr)

# Basic statistics
print("Sum:", np.sum(arr))
print("Mean:", np.mean(arr))
print("Min:", np.min(arr))
print("Max:", np.max(arr))

# Multiply all elements by 3
arr_multiplied = arr * 3
print("Array multiplied by 3:", arr_multiplied)
Key Learnings:

Arrays store multiple numbers efficiently.

NumPy can perform vectorized operations without loops.

Useful for ML datasets and calculations.

2️⃣ Pandas Exercises
python
Copy code
import pandas as pd

# Create a DataFrame
data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35],
    'Department': ['AI', 'ML', 'Data Science']
}
df = pd.DataFrame(data)

# View data
print(df.head())

# Describe numerical columns
print(df.describe())

# Filter rows: Age > 28
print(df[df['Age'] > 28])
Key Learnings:

DataFrames are like Excel spreadsheets in Python.

Can quickly summarize, filter, and explore data.

Core skill for AI pipelines.

Mini-Project: AWS + Python Workflow
Objective: Simulate analyzing a dataset and preparing it for an AI service.

Create a dataset in Pandas:

python
Copy code
dataset = {
    'ImageID': ['img1.jpg', 'img2.jpg', 'img3.jpg'],
    'Label': ['Cat', 'Dog', 'Dog'],
    'Confidence': [95, 99, 85]
}
df = pd.DataFrame(dataset)
print(df)
Convert numeric columns to NumPy arrays:

python
Copy code
confidence_array = df['Confidence'].to_numpy()
print("Confidence values as NumPy array:", confidence_array)
Calculate statistics:

python
Copy code
print("Average confidence:", np.mean(confidence_array))
print("Maximum confidence:", np.max(confidence_array))
print("Minimum confidence:", np.min(confidence_array))

