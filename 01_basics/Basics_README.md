### **1. What is Python?**

- Python is a high-level programming language used in data analysis, web development, automation, artificial intelligence, and more.

- Python is a programming language used to communicate with computers. Just like humans use English or Swahili to communicate, we use Python to give instructions to a computer.

- It is designed to be simple and easy to read, which makes it perfect for beginners. Python is used in many real-world applications such as analyzing data, building websites, automating repetitive tasks, and developing artificial intelligence systems.

- When you write Python code, you are simply telling the computer what to do step by step.

--- 

### **2. Setting Up and First Program.**
- We can run Python  in Jupyter notebook and Jupyter lab on Anaconda, IDE like pycharm, or spider or use  text edit and terminal(for a system with python interplater installed)

- The first thing beginners need to understand is that programming is about writing instructions and seeing results.

- The print() function is one of the most basic and important tools in Python. It tells the computer to display something on the screen.

When we write:

```python
print("Hello, world!")
```

> we are telling Python to show the text “Hello, world!” on the screen.

- Text in Python must be written inside quotation marks. Without quotes, Python will think it is something else and produce an error.
  
Example:

```python
print("Hello, world!")
```

**Concepts:**

- print() displays output
- Strings are written inside quotes


### **3. Variables and Data Types.**
- A variable is like a container used to store information. Instead of repeating values again and again, we store them in variables and reuse them.

Examples:
```python
name = "Harun"
age = 25
height = 1.75
is_student = True
```

**Concepts:**

- Variables store data

**- Common data types:**
        - String (text)
        - Integer (whole numbers)
        - Float (decimals)
        - Boolean (True/False)
        
### **4. Printing and Combining Data.**

-  Printing allows us to display both text and variables.

**Example 1:**

```python
name = "Harun"
print(name)
```
This prints the value stored in the variable name.

```python
print(name)
print("Hello " + name)
```
This joins the text "Hello " with the value of name. This concept is important because it allows us to create meaningful messages and outputs.

### **5. Basic Operations.**

Python can perform mathematical calculations just like a calculator. Common operations include:

- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)

**For example:**

```python
a = 10
b = 5
```

```python
print(a + b)
print(a - b)
print(a * b)
print(a / b)
```
Python calculates the result and displays it. This is useful in real-world scenarios like calculating totals, averages, or financial values.

### **6. User Input.**
Programs become more powerful when they can interact with users. The ```input()``` function allows users to enter data.

Allow programs to interact with users.

```
name = input("Enter your name: ")
print("Hello " + name)
```

**Important Note:**
>> Input is always treated as text.

### **7. Type Conversion.**

Since input is always treated as text, we sometimes need to convert it into another type.

```python
age = int(input("Enter your age: "))

```
Here, int() converts the text input into a number.

Without conversion, Python cannot perform mathematical operations on input values. Type conversion ensures that data is in the correct format for the task you want to perform.

### **8. Conditional Statements (Decision Making).**

- Conditional statements allow programs to make decisions.

**They follow a simple idea:**

>> “If something is true, do this. Otherwise, do something else.”


```python
age = int(input("Enter your age: ")

if age >= 18:
    print("You can vote")
else:
    print("You are too young")
```

**Concepts:**
- if checks a condition. 
- else runs if condition is false.
- Indentation is important.

**The program checks the condition (age >= 18):**
    - If it is true, it runs the first block
    - If it is false, it runs the second block


- Indentation (spacing) is very important in Python because it defines which code belongs inside the condition. This concept is powerful because it allows programs to behave differently based on input or conditions.

### **9. Mini Practice Exercises.**

**Exercise 1:**
- Ask for name and age, then print a message.

**Exercise 2:**
- Check if a number is even or odd.

### **10. Common Beginner Mistakes.**

- Beginners often make predictable mistakes, and addressing them early helps reduce frustration.

**Common issues include:**
- Forgetting quotation marks for text
- Incorrect indentation
- Mixing data types (e.g., adding text and numbers without conversion)
- Forgetting to convert input values

---
**You can learn more about Python from:**

1). W3Schools Python Course: https://www.w3schools.com/python/
2). Python Official Documentation: https://docs.python.org/release/3.12.0/tutorial/index.html
3). Python Community Tutorial: https://www.pythontutorial.net/

