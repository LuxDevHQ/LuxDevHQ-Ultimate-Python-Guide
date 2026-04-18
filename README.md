# Ultimate Python Guide: From Beginner to Data Analytics with NumPy, Pandas & Real Projects

Welcome to a complete, beginner-friendly, and career-focused Python learning roadmap. This guide is built to take you from **zero programming knowledge** to being able to build data-focused Python projects using:

- Core Python fundamentals
- Data analysis libraries like **NumPy** and **Pandas**
- API integration with **Requests**
- Data visualization with **Matplotlib** and **Seaborn**

Python is one of the most important programming languages today because it is:

- Easy to read and beginner-friendly
- Used in data analytics, AI/ML, web development, and automation
- Supported by a massive ecosystem of tools and libraries
- In-demand in job markets across industries

If you can read this README, you can start today.

---

## Learning Objectives

By the end of this guide, you will be able to:

1. Write clean Python programs using variables, loops, conditions, and functions.
2. Use Python data structures to organize and process information.
3. Read and write text, CSV, and JSON files.
4. Perform core statistical calculations used in analytics.
5. Analyze datasets with NumPy and Pandas.
6. Collect real-world data from APIs.
7. Create meaningful data visualizations.
8. Build portfolio-ready analytics projects.

---

## Who This Guide Is For

This guide is for:

- Complete beginners with no coding background
- Students switching to programming or analytics
- Professionals who want to automate reporting/data tasks
- Aspiring data analysts building job-ready Python skills

---

## Technologies Used

- **Python 3**
- **NumPy**
- **Pandas**
- **Requests**
- **Matplotlib**
- **Seaborn**

---

## Full Curriculum Outline

### 01. Basics
- What programming is and how Python works
- Keywords, identifiers, operators
- Variables and data types
- Input/output
- Conditions and loops

### 02. Functions
- Defining functions
- Parameters and arguments
- Return values
- Variable scope (local/global)

### 03. Data Structures
- Lists, tuples, sets, dictionaries
- Indexing and slicing
- Iteration patterns
- Comprehensions

### 04. File Handling
- Reading/writing text files
- Reading/writing CSV files
- Reading/writing JSON files

### 05. Basic Math for Analytics
- Mean, median, mode
- Variance and standard deviation
- Building reusable stats helper functions

### 06. NumPy
- Arrays and dimensions
- Vectorization
- Indexing and slicing
- Aggregations and performance patterns

### 07. Pandas
- Series and DataFrames
- Loading and inspecting datasets
- Cleaning missing/duplicate data
- Filtering and grouping

### 08. Requests & API Basics
- Making HTTP requests
- Handling status codes
- Parsing JSON responses
- Converting API data to DataFrames

### 09. Matplotlib
- Line, bar, scatter, and histogram charts
- Plot labels, titles, legends
- Basic chart formatting

### 10. Seaborn
- Statistical visualization
- Distribution plots, box plots, heatmaps
- Categorical comparisons

### 11. Real Projects
1. Data Cleaning Project (Pandas)
2. API Data + Visualization Project
3. Exploratory Data Analysis (EDA) Project

---

## Project Structure

```text
Ultimate-Python-Guide/
├── README.md
├── 01_basics/
│   └── basics_notes.py
├── 02_functions/
│   └── functions_notes.py
├── 03_data_structures/
│   └── data_structures_notes.py
├── 04_file_handling/
│   └── file_handling_notes.py
├── 05_basic_math/
│   └── basic_math_notes.py
├── 06_numpy/
│   └── numpy_notes.py
├── 07_pandas/
│   └── pandas_notes.py
├── 08_requests_api/
│   └── requests_api_notes.py
├── 09_matplotlib/
│   └── matplotlib_notes.py
├── 10_seaborn/
│   └── seaborn_notes.py
└── 11_projects/
    ├── project_1_data_cleaning.py
    ├── project_2_api_visualization.py
    └── project_3_eda.py
```

> This repository currently centralizes all teaching material in this `README.md` (as requested), while showing a recommended scalable structure.

---

## How to Use This Repository (Step-by-Step)

1. **Install Python 3.10+**
2. **Clone this repository**
   ```bash
   git clone <your-repo-url>
   cd Ultimate-Python-Guide
   ```
3. **Create virtual environment**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Linux/Mac
   .venv\Scripts\activate     # Windows
   ```
4. **Install dependencies**
   ```bash
   pip install numpy pandas requests matplotlib seaborn
   ```
5. **Read this README in order**, and run each code block.
6. **Do every practice exercise** before moving to the next module.
7. **Complete all 3 projects** and customize them with your own datasets.

---

## Contribution Guidelines

Contributions are welcome.

1. Fork the repository
2. Create a feature branch (`feature/improve-pandas-section`)
3. Make clear, tested improvements
4. Keep explanations beginner-friendly
5. Submit a Pull Request with:
   - What changed
   - Why it improves learning outcomes
   - Sample output/screenshots if relevant

Please keep tone supportive, accurate, and practical.

---

# Complete Beginner-to-Advanced Learning Guide

---

## 01_basics

### 1) Keywords
**Definition:** Keywords are reserved words in Python with special meaning (you cannot use them as variable names).

Examples: `if`, `else`, `for`, `while`, `def`, `return`, `True`, `False`, `None`.

```python
import keyword
print(keyword.kwlist[:10])
```

**Output explanation:** Prints the first 10 Python keywords from the built-in keyword list.

**Practice Exercise:**
- Write code to print the total number of keywords in Python.

---

### 2) Identifiers
**Definition:** Identifiers are names you give to variables, functions, classes, etc.

Rules:
- Can contain letters, digits, underscore
- Cannot start with a digit
- Cannot be a keyword
- Case-sensitive (`age` and `Age` are different)

```python
student_name = "Ava"
age = 21
print(student_name, age)
```

**Output explanation:** Prints the values stored in valid identifiers `student_name` and `age`.

**Practice Exercise:**
- Create 5 valid identifiers and 3 invalid ones (as comments) and explain why they are invalid.

---

### 3) Operators
**Definition:** Operators perform operations on values.

- Arithmetic: `+ - * / // % **`
- Comparison: `== != > < >= <=`
- Logical: `and or not`
- Assignment: `= += -= *=`

```python
a = 10
b = 3
print(a + b)   # 13
print(a // b)  # 3
print(a % b)   # 1
print(a > b)   # True
```

**Output explanation:** Demonstrates addition, floor division, remainder, and comparison.

**Practice Exercise:**
- Build a mini “bill calculator” using arithmetic operators.

---

### 4) Variables and Data Types

Common data types:
- `int` (whole numbers)
- `float` (decimal numbers)
- `str` (text)
- `bool` (`True/False`)

```python
name = "Sam"
score = 95
height = 5.8
is_passed = True

print(type(name), type(score), type(height), type(is_passed))
```

**Output explanation:** Shows each variable's data type using `type()`.

**Practice Exercise:**
- Create a profile card using 6 variables of different data types.

---

### 5) Input and Output

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))
print(f"Hello {name}, next year you will be {age + 1}.")
```

**Output explanation:** Takes user input, converts age to integer, and prints a formatted message.

**Practice Exercise:**
- Create a script that asks for 3 subject marks and prints total and average.

---

### 6) Conditions

```python
temperature = 30
if temperature > 35:
    print("Very hot")
elif temperature >= 25:
    print("Warm")
else:
    print("Cool")
```

**Output explanation:** Python evaluates conditions top-down and runs the first true block.

**Practice Exercise:**
- Build grade classification (`A/B/C/Fail`) from score.

---

### 7) Loops

```python
# for loop
for i in range(1, 6):
    print(i)

# while loop
count = 3
while count > 0:
    print("Countdown:", count)
    count -= 1
```

**Output explanation:** `for` repeats over a range, `while` repeats while condition remains true.

**Practice Exercise:**
- Print multiplication table of any number from 1 to 10.

---

## 02_functions

### 1) Function Definition
**Analogy:** A function is like a kitchen recipe—same instructions, reusable anytime.

```python
def greet():
    print("Welcome to Python learning!")

greet()
```

**Output explanation:** Calling `greet()` executes the code inside the function.

**Practice Exercise:**
- Write a function that prints your learning goal.

---

### 2) Parameters and Arguments

```python
def greet_user(name):
    print(f"Hello, {name}!")

greet_user("Nina")
```

**Output explanation:** `name` is a parameter; `"Nina"` is the argument passed at call time.

**Practice Exercise:**
- Create `calculate_area(length, width)` and print rectangle area.

---

### 3) Return Values

```python
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 7)
print(result)
```

**Output explanation:** `return` sends value back to caller for reuse.

**Practice Exercise:**
- Write `is_even(number)` returning `True`/`False`.

---

### 4) Scope (Local vs Global)

```python
x = "global"

def show_scope():
    x = "local"
    print("Inside:", x)

show_scope()
print("Outside:", x)
```

**Output explanation:** Local variable exists only inside function; global remains unchanged.

**Practice Exercise:**
- Create a counter function and observe local variable reset behavior.

---

## 03_data_structures

### 1) Lists
Ordered, mutable collection.

```python
fruits = ["apple", "banana", "cherry"]
fruits.append("mango")
print(fruits)
print(fruits[1])
```

**Output explanation:** `append` adds item; indexing starts at 0.

**Practice Exercise:**
- Store 5 expenses in a list and print total.

---

### 2) Tuples
Ordered, immutable collection.

```python
coordinates = (10.5, 20.3)
print(coordinates[0])
```

**Output explanation:** Tuple values are fixed once created.

**Practice Exercise:**
- Create tuple of weekdays and print third day.

---

### 3) Sets
Unordered, unique values only.

```python
ids = {101, 102, 102, 103}
print(ids)
```

**Output explanation:** Duplicate `102` appears once because sets enforce uniqueness.

**Practice Exercise:**
- Convert a list with duplicates to set and back to list.

---

### 4) Dictionaries
Key-value mapping.

```python
student = {"name": "Ivy", "score": 88}
print(student["name"])
student["passed"] = True
print(student)
```

**Output explanation:** Dictionary access happens by keys, not numeric index.

**Practice Exercise:**
- Build a dictionary for product info: name, price, quantity.

---

### 5) Comprehensions
Compact way to create collections.

```python
squares = [n * n for n in range(1, 6)]
print(squares)

even_squares = [n * n for n in range(1, 11) if n % 2 == 0]
print(even_squares)
```

**Output explanation:** Creates lists by combining loops + optional conditions in one line.

**Practice Exercise:**
- Create dictionary comprehension mapping number to cube from 1 to 5.

---

## 04_file_handling

### 1) Text Files

```python
with open("notes.txt", "w") as f:
    f.write("Python is powerful.\n")

with open("notes.txt", "r") as f:
    content = f.read()
print(content)
```

**Output explanation:** Writes to file, then reads full content. `with` auto-closes file safely.

**Practice Exercise:**
- Write 3 lines to `todo.txt`, then read them line-by-line.

---

### 2) CSV Files

```python
import csv

rows = [
    ["name", "score"],
    ["Ana", 91],
    ["Ben", 85]
]

with open("scores.csv", "w", newline="") as f:
    writer = csv.writer(f)
    writer.writerows(rows)

with open("scores.csv", "r") as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)
```

**Output explanation:** Writes tabular data and reads it row by row.

**Practice Exercise:**
- Create a CSV of monthly expenses and compute total.

---

### 3) JSON Files

```python
import json

data = {"city": "New York", "temp": 24, "unit": "C"}

with open("weather.json", "w") as f:
    json.dump(data, f, indent=2)

with open("weather.json", "r") as f:
    loaded = json.load(f)
print(loaded["city"])
```

**Output explanation:** JSON stores structured data; `dump` writes, `load` reads.

**Practice Exercise:**
- Save a small student record in JSON and read it back.

---

## 05_basic_math

```python
import statistics as stats

data = [10, 12, 12, 15, 18]

print("Mean:", stats.mean(data))
print("Median:", stats.median(data))
print("Mode:", stats.mode(data))
print("Variance:", stats.pvariance(data))
print("Standard Deviation:", stats.pstdev(data))
```

**Output explanation:**
- Mean: average value
- Median: middle value in sorted data
- Mode: most frequent value
- Variance: spread from mean (squared)
- Standard deviation: spread in original units

**Practice Exercise:**
- Create a function that accepts a list and returns all 5 statistics in a dictionary.

---

## 06_numpy

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr * 2)                 # vectorization
print(arr[1:4])                # indexing/slicing
print(np.mean(arr), np.std(arr))
```

**Output explanation:**
- Vectorization applies operation to all elements without explicit loops.
- Slicing extracts a subset efficiently.
- NumPy aggregations are fast and concise.

**Practice Exercise:**
- Create 3x3 array and calculate row-wise sums.

---

## 07_pandas

```python
import pandas as pd

df = pd.DataFrame({
    "name": ["A", "B", "C", "D"],
    "age": [23, 35, None, 29],
    "salary": [50000, 62000, 58000, None],
    "dept": ["IT", "HR", "IT", "Sales"]
})

print(df.head())
print(df.isna().sum())

clean_df = df.dropna()
it_staff = clean_df[clean_df["dept"] == "IT"]
summary = clean_df.groupby("dept")["salary"].mean()

print(it_staff)
print(summary)
```

**Output explanation:**
- Builds DataFrame
- Detects missing values
- Removes incomplete rows
- Filters only IT department
- Groups by department and computes mean salary

**Practice Exercise:**
- Load a CSV and calculate average score by class.

---

## 08_requests_api

```python
import requests
import pandas as pd

url = "https://jsonplaceholder.typicode.com/posts"
response = requests.get(url, timeout=10)

if response.status_code == 200:
    data = response.json()
    df = pd.DataFrame(data)
    print(df[["userId", "id", "title"]].head())
else:
    print("Request failed with status:", response.status_code)
```

**Output explanation:**
- Calls public API endpoint
- Checks status code
- Parses JSON response
- Converts response into DataFrame for analysis

**Practice Exercise:**
- Fetch users endpoint and print user names + emails.

---

## 09_matplotlib

```python
import matplotlib.pyplot as plt

months = ["Jan", "Feb", "Mar", "Apr"]
sales = [1200, 1500, 1700, 1600]

plt.plot(months, sales, marker="o")
plt.title("Monthly Sales")
plt.xlabel("Month")
plt.ylabel("Revenue")
plt.grid(True)
plt.show()
```

**Output explanation:** Creates line chart to show sales trend across months.

**Practice Exercise:**
- Build a bar chart comparing product sales.

---

## 10_seaborn

```python
import seaborn as sns
import matplotlib.pyplot as plt
import pandas as pd

df = pd.DataFrame({
    "department": ["IT", "IT", "HR", "HR", "Sales", "Sales"],
    "salary": [60000, 65000, 52000, 54000, 50000, 58000]
})

sns.boxplot(data=df, x="department", y="salary")
plt.title("Salary Distribution by Department")
plt.show()
```

**Output explanation:** Boxplot shows median, quartiles, spread, and potential outliers by department.

**Practice Exercise:**
- Create `sns.histplot()` for customer ages and interpret skew.

---

## 11_projects (MANDATORY)

## Project 1: Data Cleaning Project (Pandas)

### Problem Statement
You received raw employee data with missing values, duplicates, and inconsistent text formatting. Clean the data and generate a summary for reporting.

### Step-by-Step Solution

```python
import pandas as pd

# Step 1: Simulated raw data
raw_data = pd.DataFrame({
    "employee_id": [1, 2, 2, 3, 4],
    "name": ["alice", "BOB", "BOB", "Charlie", None],
    "department": ["it", "HR", "HR", "sales", "IT"],
    "salary": [60000, None, None, 52000, 58000]
})

# Step 2: Remove duplicates
df = raw_data.drop_duplicates()

# Step 3: Standardize text
df["name"] = df["name"].fillna("Unknown").str.title()
df["department"] = df["department"].str.upper()

# Step 4: Fill missing salary with department median
df["salary"] = df.groupby("department")["salary"].transform(
    lambda s: s.fillna(s.median())
)

# Step 5: Final summary
summary = df.groupby("department")["salary"].agg(["count", "mean", "min", "max"])

print("Cleaned Data:\n", df)
print("\nDepartment Salary Summary:\n", summary)
```

### What You Learn
- Deduplication
- Missing value handling
- Text normalization
- Grouped aggregation for reporting

---

## Project 2: API Data + Visualization Project

### Problem Statement
Collect live-like data from an API and visualize useful trends for stakeholders.

### Step-by-Step Solution

```python
import requests
import pandas as pd
import matplotlib.pyplot as plt

# Step 1: Fetch data
url = "https://jsonplaceholder.typicode.com/todos"
resp = requests.get(url, timeout=10)
resp.raise_for_status()
data = resp.json()

# Step 2: Convert to DataFrame
df = pd.DataFrame(data)

# Step 3: Engineer simple metric
completion = df.groupby("userId")["completed"].mean() * 100

# Step 4: Plot
completion.sort_values().plot(kind="bar", figsize=(10, 5), color="teal")
plt.title("Task Completion Rate by User (%)")
plt.xlabel("User ID")
plt.ylabel("Completion Rate (%)")
plt.tight_layout()
plt.show()

print(completion.round(2))
```

### What You Learn
- API ingestion
- DataFrame transformation
- Creating a decision-friendly chart

---

## Project 3: Exploratory Data Analysis (EDA) Project

### Problem Statement
Analyze retail transaction data to find top products, monthly sales trends, and customer behavior patterns.

### Step-by-Step Solution

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Step 1: Sample dataset
sales = pd.DataFrame({
    "date": pd.to_datetime([
        "2026-01-05", "2026-01-17", "2026-02-03", "2026-02-11", "2026-03-09", "2026-03-21"
    ]),
    "product": ["Laptop", "Mouse", "Laptop", "Keyboard", "Mouse", "Laptop"],
    "units": [3, 10, 2, 5, 8, 4],
    "unit_price": [900, 25, 920, 45, 25, 910]
})

# Step 2: Feature engineering
sales["revenue"] = sales["units"] * sales["unit_price"]
sales["month"] = sales["date"].dt.to_period("M").astype(str)

# Step 3: Core EDA metrics
monthly_revenue = sales.groupby("month")["revenue"].sum()
product_revenue = sales.groupby("product")["revenue"].sum().sort_values(ascending=False)

print("Monthly Revenue:\n", monthly_revenue)
print("\nProduct Revenue:\n", product_revenue)

# Step 4: Visualize
plt.figure(figsize=(8, 4))
sns.barplot(x=product_revenue.index, y=product_revenue.values)
plt.title("Revenue by Product")
plt.xlabel("Product")
plt.ylabel("Revenue")
plt.tight_layout()
plt.show()
```

### What You Learn
- EDA workflow
- Feature engineering
- Grouped business insights
- Visualization for storytelling

---

## Learning Path Milestones (Zero → Job-Ready)

- **Stage 1 (Weeks 1–2):** Python basics + functions
- **Stage 2 (Weeks 3–4):** Data structures + file handling + math
- **Stage 3 (Weeks 5–6):** NumPy + Pandas
- **Stage 4 (Week 7):** APIs + Visualization
- **Stage 5 (Week 8):** Complete and polish all projects

Portfolio tip: Push project notebooks/scripts to GitHub with screenshots and concise business conclusions.

---

## Final Notes

This guide is intentionally structured as a practical curriculum instead of isolated theory. If you run every code block, complete every exercise, and finish the 3 projects, you will build real confidence with Python for analytics roles.

Consistency beats intensity. Study daily, even if only 45 minutes.
