### **Intermediate Python: Loops, Conditional Statements & User-Defined Functions**

---

## **1. Loops in Python**
Loops are one of the most important concepts in programming. They allow your program to repeat actions automatically, instead of writing the same code multiple times.

Think of a loop like this:

>> If you had to greet 100 students one by one, would you write 100 print statements?
No. You use a loop to do it for you.

**Why Do We Use Loops?**

Loops help us:
- Save time (write less code)
- Avoid repetition (Don’t Repeat Yourself – DRY principle)
- Work with large datasets (lists, tables, files)
- Automate tasks

**Real-Life Analogy**

Imagine a teacher taking attendance:
- The teacher calls one name at a time → this is like a loop
- The list of students → this is the sequence
- The action (marking present) → this is the loop body

**How Loops Work.**

A loop follows this pattern:
    1). Start.
    2). Check condition or pick next item.
    3). Execute code.
    4). Repeat until condition is false or items are finished.

### **Types of Loops**
- `for` loop → used when you know the number of iterations  
- `while` loop → used when the number of iterations depends on a condition  

---

### **1.1 For Loop**

A `for` loop iterates over a sequence (list, tuple, string, range, etc.)

#### **Basic Example**
```python
for i in range(5):
    print(i)
```

#### **Looping Through a List**
```python
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)
```

#### **Looping Through a String**
```python
name = "LuxDevHQ"

for char in name:
    print(char)
```

#### **Using range()**
```python
for i in range(1, 6):
    print(i)
```

#### **Using Step in range()**
```python
for i in range(0, 10, 2):
    print(i)
```

---

### **1.2 While Loop**

Executes as long as a condition is `True`.

```python
count = 0

while count < 5:
    print(count)
    count += 1
```

---

### **1.3 Break and Continue**

#### **Break (Stop Loop)**
```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

#### **Continue (Skip Iteration)**
```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

---

### **1.4 Nested Loops**

A loop inside another loop.

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```

---

## **2. Conditional Statements**

Used to make decisions in your code.

### **2.1 Basic If Statement**
```python
age = 18

if age >= 18:
    print("You are an adult")
```

### **2.2 If-Else**
```python
age = 16

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

### **2.3 If-Elif-Else**
```python
marks = 75

if marks >= 80:
    print("A")
elif marks >= 60:
    print("B")
elif marks >= 50:
    print("C")
else:
    print("Fail")
```

### **2.4 Logical Operators**
```python
age = 20
has_id = True

if age >= 18 and has_id:
    print("Allowed entry")
```

### **2.5 Comparison Operators**
```python
x = 10

if x != 5:
    print("x is not 5")
```

### **2.6 Nested Conditionals**
```python
age = 25
income = 50000

if age > 18:
    if income > 30000:
        print("Eligible for loan")
```

---

## **3. User-Defined Functions**

Functions allow you to group code into reusable blocks.

### **3.1 Creating a Function**
```python
def greet():
    print("Hello, welcome to LuxDevHQ!")
```

### **3.2 Calling a Function**
```python
greet()
```

### **3.3 Function with Parameters**
```python
def greet(name):
    print("Hello", name)

greet("Harun")
```

### **3.4 Function with Return Value**
```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)
```

### **3.5 Default Parameters**
```python
def greet(name="Guest"):
    print("Hello", name)

greet()
greet("LuxDevHQ")
```

### **3.6 Multiple Parameters**
```python
def student_info(name, age, course):
    print(name, age, course)

student_info("John", 22, "Data Science")
```

### **3.7 Keyword Arguments**
```python
def student_info(name, age):
    print(name, age)

student_info(age=25, name="Alice")
```

### **3.8 Combining Loops + Functions**
```python
def print_numbers(n):
    for i in range(n):
        print(i)

print_numbers(5)
```

### **3.9 Function with Conditionals**
```python
def check_even(number):
    if number % 2 == 0:
        return "Even"
    else:
        return "Odd"

print(check_even(4))
```

---

## **4. Real-Life Example (Mini Project)**

### **Student Grade System**
```python
def calculate_grade(score):
    if score >= 80:
        return "A"
    elif score >= 60:
        return "B"
    elif score >= 50:
        return "C"
    else:
        return "Fail"

students = [85, 67, 45, 90]

for score in students:
    print(score, calculate_grade(score))
```

---

## **5. Practice Exercises**

1. Print numbers from 1–20 using a loop  
2. Write a function that checks if a number is prime  
3. Create a grading system using conditionals  
4. Loop through a list of names and print greetings  
5. Write a function that returns the largest of 3 numbers  
