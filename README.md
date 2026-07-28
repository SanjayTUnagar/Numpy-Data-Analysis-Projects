# 🔢 NumPy — Numerical Computing Library

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-orange?logo=numpy)
![IBM Certification](https://img.shields.io/badge/IBM-Data%20Visualization%20with%20Python-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

# 📖 Overview

**NumPy (Numerical Python)** is one of the most important libraries in Python for numerical and scientific computing.

It provides a powerful **ndarray (N-dimensional array)** object that allows developers and data analysts to perform mathematical operations on large datasets efficiently.

Compared to traditional Python lists, NumPy arrays are:

⚡ Faster in computation

 💾 More memory efficient
 
 📊 Optimized for numerical operations
 
 🔄 Designed for vectorized calculations

NumPy is the foundation of many popular Python data libraries including:

🐼 Pandas

📈 Matplotlib

🤖 Scikit-learn

🧠 TensorFlow

---

# ⚙️ Installation

Install NumPy using pip:

```bash
pip install numpy
```

Verify installation:

```python
import numpy as np

print(np.__version__)
```

---

# 🚀 Getting Started with NumPy

## Import NumPy

```python
import numpy as np
```

---

# 📌 Basic NumPy Array Example

```python
import numpy as np

numbers = np.array([10, 20, 30, 40, 50])

print("Array:", numbers)
print("Mean:", numbers.mean())
print("Maximum:", numbers.max())
print("Doubled:", numbers * 2)
```

### Output

```
Array: [10 20 30 40 50]

Mean: 30.0

Maximum: 50

Doubled:
[ 20  40  60  80 100 ]
```

---

# 📚 NumPy Array Features Demonstrated

| Function | Description |
|---|---|
| `np.array()` | Creates NumPy array |
| `.mean()` | Calculates average value |
| `.max()` | Finds maximum value |
| `.min()` | Finds minimum value |
| Array Multiplication | Performs vectorized operations |

---

# 🚀 Mini Project

# 🎓 Student Score Analyzer

## Project Objective

The goal of this mini project is to analyze student examination scores using only NumPy.

The program performs:

✅ Average score calculation  
✅ Highest and lowest score detection  
✅ Standard deviation calculation  
✅ Median calculation  
✅ Percentile analysis  
✅ Pass/Fail classification  
✅ Grade distribution analysis  

---

# 📝 Project Workflow

```
Student Scores Dataset
          |
          ↓
Create NumPy Array
          |
          ↓
Statistical Analysis
          |
          ↓
Pass / Fail Classification
          |
          ↓
Grade Calculation
          |
          ↓
Final Report
```

---

# 💻 Project Code

```python
import numpy as np


# Step 1: Generate Student Scores
# 30 students marks out of 100

np.random.seed(10)

scores = np.random.randint(40, 100, 30)


# Step 2: Basic Statistics

print("All Scores:", scores)

print("Average Score:",
      round(scores.mean(), 2))

print("Highest Score:",
      scores.max())

print("Lowest Score:",
      scores.min())

print("Standard Deviation:",
      round(scores.std(), 2))

print("Median Score:",
      np.median(scores))


# Step 3: Percentile Analysis

print("\n75th Percentile:",
      np.percentile(scores,75))

print("25th Percentile:",
      np.percentile(scores,25))


# Step 4: Pass / Fail Classification

passed = scores[scores >= 50]

failed = scores[scores < 50]


print("\nStudents Passed:",
      len(passed))


print("Students Failed:",
      len(failed))


print("Pass Percentage:",
      round(len(passed)/len(scores)*100,1),
      "%")


# Step 5: Grade Distribution

grades = np.where(scores >= 90,"A",
          np.where(scores >= 75,"B",
          np.where(scores >= 60,"C",
          np.where(scores >= 50,"D","F"))))


unique, counts = np.unique(
    grades,
    return_counts=True
)


print("\nGrade Distribution:")

for grade,count in zip(unique,counts):
    print(
        f"{grade}: {count} students"
    )
```

---

# 📊 Sample Output

```
All Scores:
[49 85 64 40 73 55 98 42 88 61]


Average Score: 68.43

Highest Score: 98

Lowest Score: 40

Standard Deviation: 17.32

Median Score: 69


75th Percentile: 84.75

25th Percentile: 55.0


Students Passed: 27

Students Failed: 3

Pass Percentage: 90.0%


Grade Distribution:

A: 5 students

B: 8 students

C: 10 students

D: 4 students

F: 3 students
```

---

# 🧠 Concepts Covered

| Concept | NumPy Feature |
|---|---|
| Array Creation | `np.array()` |
| Random Data Generation | `np.random.randint()` |
| Average Calculation | `mean()` |
| Maximum Value | `max()` |
| Minimum Value | `min()` |
| Standard Deviation | `std()` |
| Median | `median()` |
| Percentile | `percentile()` |
| Filtering Data | Boolean Masking |
| Conditional Logic | `np.where()` |
| Frequency Count | `np.unique()` |

---

# 📂 Project Structure

```
NumPy-Student-Score-Analyzer/
│
├── README.md
│
├── student_score_analyzer.py
│
└── requirements.txt
```

---

# 📦 Requirements

Create `requirements.txt`

```
numpy
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# 🎯 Learning Outcomes

After completing this project, you will understand:

✔ NumPy array creation  
✔ Numerical computation techniques  
✔ Statistical data analysis  
✔ Data filtering using arrays  
✔ Conditional operations  
✔ Working with random datasets  
✔ Foundation of Data Analytics using Python  

---

# 🌍 Real-World Applications

NumPy is used in:

- 📊 Data Analytics
- 🤖 Machine Learning
- 🧬 Scientific Research
- 💹 Financial Modeling
- 🖼 Image Processing
- 📈 Data Visualization
- 🏭 Engineering Simulations

---

# 🏆 Certification Reference

This project is part of the learning journey for:

**IBM — Data Visualization with Python (DV0101EN)**

Topics Covered:

- Python Data Analysis
- NumPy Fundamentals
- Data Manipulation
- Visualization Preparation

---

# 👨‍💻 Author

**Sanjay Unagar**

Data Analyst | Python | SQL | Excel | Power BI | Data Visualization

🔗 GitHub:  
https://github.com/SanjayTUnagar

🔗 LinkedIn:  
https://www.linkedin.com/in/sanjayunagar/

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

---

# 📌 Conclusion

NumPy is the backbone of Python numerical computing.  
Mastering NumPy arrays and operations provides the foundation required for advanced Data Analytics, Machine Learning, and Artificial Intelligence projects.
