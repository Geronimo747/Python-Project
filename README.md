# Python-Project
# 🐍 Python Fundamentals Project Portfolio

## 📖 Overview

This repository contains my completed Python exercises from the Data Technician Week 6 Workbook. The project focused on building practical programming skills through real-world scenarios and problem-solving activities.

Throughout these exercises, I developed programs using core Python concepts including:

- ✅ Variables and data types
- ✅ User input and output
- ✅ Mathematical calculations
- ✅ Conditional statements (`if`, `elif`, `else`)
- ✅ Loops (`for` and `while`)
- ✅ Input validation
- ✅ String manipulation
- ✅ Floor division (`//`) and modulus (`%`)
- ✅ Problem-solving and debugging

These tasks helped strengthen my understanding of Python fundamentals and demonstrated how programming can be used to solve everyday business and customer-focused challenges. 【1-9e39f0】

---

# 📅 Day 1 - Python Basics

## 🏢 Community Centre Reception System
Created a visitor registration program that:

- Collects a visitor's name and age
- Displays a personalised greeting
- Provides eligibility information based on age

### Skills Used
- User input
- Variables
- String formatting

---

## 🏠 Kitchen Tile Calculator
Developed a program that:

- Accepts kitchen length and width
- Calculates total floor area
- Calculates tile cost based on price per square metre

### Skills Used
- Float data types
- Mathematical calculations
- Formatted output

---

## 🌡️ Temperature Converter
Built a temperature conversion tool that:

- Converts Celsius to Fahrenheit
- Converts Fahrenheit to Celsius
- Includes input validation and menu options

### Skills Used
- Mathematical formulas
- While loops
- Input validation
- Conditional statements

---

## 🛣️ Distance Converter
Created a distance conversion application that:

- Converts Miles ➜ Kilometres
- Converts Kilometres ➜ Miles
- Allows the user to perform multiple conversions

### Skills Used
- Loops
- User interaction
- Mathematical calculations

---

## 🍀 Lucky Number Generator
Designed a fun program that:

- Accepts a 3-digit number
- Separates individual digits
- Calculates the sum of the digits

### Skills Used
- Floor division (`//`)
- Modulus operator (`%`)
- Integer arithmetic

---

## 🔐 Secret Code Reverser
Developed a puzzle-solving tool that:

- Accepts a 4-digit number
- Extracts individual digits
- Reverses the number to create a secret code

### Skills Used
- Digit extraction
- Number manipulation
- Mathematical logic

---

# 📅 Day 2 - Decision Making & Loops

## 🔒 Security Door Access System
Created a login system that:

- Checks a user-entered security code
- Grants or denies access
- Locks the account after multiple failed attempts

### Skills Used
- While loops
- Authentication logic
- Conditional statements

---

## 🔢 Divisibility Checker
Built a maths utility that:

- Checks if a number is divisible by both 3 and 7
- Displays clear feedback to the user

### Skills Used
- Modulus operator (`%`)
- Boolean logic

---

## 🧮 Menu-Driven Calculator
Developed an interactive calculator capable of:

- Addition
- Subtraction
- Multiplication
- Division
- Exit functionality

### Skills Used
- Menu systems
- Loops
- Conditional statements
- Error handling

---

## 👟 Fitness Tracker Sum Calculator
Created a program that:

- Calculates the total sum from 1 to a chosen number
- Simulates increasing daily fitness goals

### Skills Used
- For loops
- Accumulators
- Mathematical calculations

---

## 🔍 Prime Number Checker
Designed a program that:

- Determines whether a number is prime
- Displays an appropriate result

### Skills Used
- Loops
- Decision making
- Number theory

---

## ✖️ Factorial Calculator
Built a factorial calculation tool that:

- Accepts a non-negative integer
- Calculates the factorial value

### Skills Used
- Iteration
- Mathematical problem solving

---

## 📐 Number Pattern Generator
Created a staircase pattern generator using nested loops:

<img width="260" height="171" alt="image" src="https://github.com/user-attachments/assets/c2445274-993d-41bf-8d42-fde7e8773cd2" />

---

## 🧩 Bonus Challenge: FizzBuzz

One of the most common beginner programming challenges is **FizzBuzz**, which tests the use of loops, conditional statements, and the modulus operator.

### 🎯 Objective

Create a program that loops through numbers from **1 to 100** and:

- Prints **"Fizz"** if the number is divisible by 3
- Prints **"Buzz"** if the number is divisible by 5
- Prints **"FizzBuzz"** if the number is divisible by both numbers
- Otherwise prints the number itself

### 💻 Python Solution

```python
fizzbuzz = input("Enter a number: ")
fizzbuzz = int(fizzbuzz)
while
if fizzbuzz % 3 == 0 and fizzbuzz % 7 == 0:
  print("fizzbuzz")
elif fizzbuzz % 3 == 0:
  print("fizz")
elif fizzbuzz % 7 == 0:
  print("buzz")
