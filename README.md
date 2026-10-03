# 🐍 Python Programming Lab: Iterative Control Flow & Loops (Task 02)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/islamyasser424-design/python-task-02.ipynb/blob/main/python_task_02.ipynb)
![Python Version](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Topics](https://img.shields.io/badge/Focus-Control%20Flow%20%26%20Loops-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A comprehensive Python laboratory assignment focusing on fundamental iteration paradigms, algorithmic control flow, nested structures, loop interruption protocols (`break`, `continue`), and function placeholders (`pass`).

---

## 📌 Table of Contents
- [📖 Overview](#-overview)
- [🎯 Learning Objectives](#-learning-objectives)
- [🧩 Problem Statements & Solutions](#-problem-statements--solutions)
  - [1. Definite Iteration: `for` Loop](#1-definite-iteration-for-loop)
  - [2. State-Driven Iteration: `while` Loop](#2-state-driven-iteration-while-loop)
  - [3. Multi-Dimensional Grid: Nested Loops](#3-multi-dimensional-grid-nested-loops)
  - [4. Interactive Sentinel Accumulator: `while True` & `break`](#4-interactive-sentinel-accumulator-while-true--break)
  - [5. Conditional Value Skipping: `continue`](#5-conditional-value-skipping-continue)
  - [6. Function Structural Stub: `pass`](#6-function-structural-stub-pass)
- [📊 Summary Matrix](#-summary-matrix)
- [💻 Getting Started & Execution](#-getting-started--execution)
- [👤 Author & Connect](#-author--connect)

---

## 📖 Overview

Mastering iterative constructs and loop execution controls is essential for algorithmic problem-solving and data analysis in Python. This repository contains solutions to foundational programming challenges designed to solidify understanding of:
- **Sequential range iteration** using finite `for` loops.
- **Conditional state-checking** using dynamic `while` loops.
- **Two-dimensional coordinate traversal** with nested loops.
- **Execution interruption** via `break` upon reaching a user-defined sentinel value.
- **Selective cycle bypass** using `continue`.
- **Modular scaffolding** with the syntactically required `pass` statement.

---

## 🎯 Learning Objectives

* Understand the mechanical differences between definite iteration (`for`) and indefinite iteration (`while`).
* Control iteration boundaries and step logic using Python's built-in `range()` function.
* Construct nested iterative matrices for geometric and tabular pattern generation.
* Prevent infinite loops while managing dynamic, user-driven inputs through break conditions.
* Leverage `continue` for clean filtering without nested branching.
* Utilize `pass` to design modular function signatures and interface stubs without triggering indentation errors.

---

## 🧩 Problem Statements & Solutions

### 1. Definite Iteration: `for` Loop
**Prompt:** Write a program that prints all the numbers from 1 to 10 using a `for` loop.

```python
for x in range(1, 11):
    print(x)
```
* **Mechanism:** Utilizes `range(1, 11)` where the lower bound is inclusive (`1`) and the upper bound is exclusive (`11`), generating a deterministic sequence of 10 integers.
* **Output:**
```text
1
2
3
...
10
```

---

### 2. State-Driven Iteration: `while` Loop
**Prompt:** Write a program that prints all the numbers from 1 to 10 using a `while` loop.

```python
num = 1

while num <= 10:
    print(num)
    num = num + 1
```
* **Mechanism:** Initializes a state variable `num = 1`, evaluates the boolean guard condition `num <= 10` before each iteration, and increments the counter deterministically to guarantee loop termination.

---

### 3. Multi-Dimensional Grid: Nested Loops
**Prompt:** Write a program that prints a 5x5 grid of asterisks (`*`) using nested loops.

```python
for i in range(5):
    for j in range(5):
        print("*", end=" ")
    print()
```
* **Mechanism:** The outer loop controls rows (5 iterations), while the inner loop controls columns (5 iterations). Using `end=" "` retains the horizontal print head, and `print()` executes a line break at the end of each row.
* **Output:**
```text
* * * * * 
* * * * * 
* * * * * 
* * * * * 
* * * * * 
```

---

### 4. Interactive Sentinel Accumulator: `while True` & `break`
**Prompt:** Write a program that asks the user to input numbers until they input `0`. The program should print the sum of all the input numbers.

```python
total = 0

while True:
    num = int(input("Enter a number: "))

    if num == 0:
        break

    total = total + num

print("Sum =", total)
```
* **Mechanism:** Implements an intentional indefinite loop (`while True`) guarded by a sentinel check (`num == 0`). Once the sentinel is encountered, `break` immediately terminates the loop without adding `0` to the accumulator.

---

### 5. Conditional Value Skipping: `continue`
**Prompt:** Write a program that prints all the numbers from 1 to 10 except 5 using a `for` loop and `continue` statement.

```python
for i in range(1, 11):
    if i == 5:
        continue
    print(i)
```
* **Mechanism:** When `i == 5`, the `continue` keyword immediately halts the current iteration, bypasses the subsequent `print(i)` call, and advances the loop counter to `6`.
* **Output:**
```text
1
2
3
4
6
7
8
9
10
```

---

### 6. Function Structural Stub: `pass`
**Prompt:** Write a program that defines an empty function using the `pass` statement.

```python
def my_function():
    pass
```
* **Mechanism:** Python requires an indented block after function definitions (`def`). The `pass` keyword acts as a syntactically valid null operation (NOP), allowing developers to scaffold interfaces and architecture without syntax errors.

---

## 📊 Summary Matrix

| # | Task | Control Structure | Primary Keyword | Complexity | Use Case |
|---|------|-------------------|-----------------|------------|----------|
| **1** | Sequential Print | Definite Loop | `for`, `range()` | $\mathcal{O}(N)$ | Predictable sequence processing |
| **2** | Conditional Counter | Indefinite Loop | `while`, `<=` | $\mathcal{O}(N)$ | State-dependent processing |
| **3** | 2D Asterisk Matrix | Nested Loops | `for in for` | $\mathcal{O}(N \times M)$ | Matrix traversal, spatial graphics |
| **4** | Sentinel Summation | Event-Driven Loop | `while True`, `break` | Dynamic | User inputs, stream ingestion |
| **5** | Number Filter | Selective Loop | `continue` | $\mathcal{O}(N)$ | Data cleansing, anomaly filtering |
| **6** | Function Stub | Architecture Stub | `pass` | $\mathcal{O}(1)$ | Code scaffolding, modular blueprints |

---

## 💻 Getting Started & Execution

### Option 1: Run Online in Google Colab (Zero Setup)
Click the badge below to execute and experiment with the notebook directly in your browser:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/islamyasser424-design/python-task-02.ipynb/blob/main/python_task_02.ipynb)

### Option 2: Run Locally via Git & Jupyter

1. **Clone the repository:**
   ```bash
   git clone https://github.com/islamyasser424-design/python-task-02.ipynb.git
   cd python-task-02.ipynb
   ```

2. **Set up a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Jupyter and launch:**
   ```bash
   pip install jupyterlab notebook
   jupyter notebook python_task_02.ipynb
   ```

---

## 👤 Author & Connect

**Islam Yasser**  
*Data Analyst & Business Intelligence Specialist*

* 🌐 **Portfolio Website:** [islamyasser424-design.github.io/portfolio-](https://islamyasser424-design.github.io/portfolio-/)
* 💼 **LinkedIn:** [linkedin.com/in/islam-yasser-55048b378](https://www.linkedin.com/in/islam-yasser-55048b378/)
* 🐙 **GitHub Profile:** [@islamyasser424-design](https://github.com/islamyasser424-design)
* ✉️ **Email:** [islamyasser424@gmail.com](mailto:islamyasser424@gmail.com)

---
<p align="center">
  <sub>Part of the Python Programming & Data Analytics Portfolio series. Built with precision and clean code standards.</sub>
</p>