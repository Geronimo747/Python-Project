# Python-Project
# <img width="48" height="48" alt="image" src="https://github.com/user-attachments/assets/84ac4126-4898-4501-b24e-48ce48785eeb" /> Python Fundamentals Project Portfolio

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

These tasks helped strengthen my understanding of Python fundamentals and demonstrated how programming can be used to solve everyday business and customer-focused challenges. 

---

# Day 1 - Python Basics

## Community Centre Reception System
Created a visitor registration program that:

- Collects a visitor's name and age
- Displays a personalised greeting
- Provides eligibility information based on age

## Skills Used
- User input
- Variables
- String formatting

```python
print("Hello Guest\n")
Name = input("Please Provide Name: ")
Age = input("Please Provide Age: ")
print("Hello",Name,"\b, welcome to the Community Centre! At",Age,"\b, you're eligible for our young adults programe.")
```     
Hello Guest

Please Provide Name: Geronimo
Please Provide Age: 29
Hello Geronimo , welcome to the Community Centre! At 29 ,you're eligible for our young adults programe.

---

## Kitchen Tile Calculator
Developed a program that:

- Accepts kitchen length and width
- Calculates total floor area
- Calculates tile cost based on price per square metre

## Skills Used
- Float data types
- Mathematical calculations
- Formatted output

```python
print("Enter The Length and Width of Kitchen\n")

A_str = input("Enter a Width of kitchen in metres: ")
B_str = input("Enter a Length of kitchen in metres ")

try:
    # Convert inputs to integers for numerical addition
    A = float(A_str)
    B = float(B_str)
    area = A * B # Use a different variable name for the area
    cost = area * 12
    print(f"You will need {area} square meteres of tiles.\nThe total cost will be £{cost}") # Use print as a function
except ValueError:
    print("Invalid input. Please enter valid numbers.")
``` 
     
Enter The Length and Width of Kitchen

Enter a Width of kitchen in metres: 3.5
Enter a Length of kitchen in metres 2.8
You will need 9.799999999999999 square meteres of tiles.
The total cost will be £117.6

---

## 🌡️ Temperature Converter
Built a temperature conversion tool that:

- Converts Celsius to Fahrenheit
- Converts Fahrenheit to Celsius
- Includes input validation and menu options

## Skills Used
- Mathematical formulas
- While loops
- Input validation
- Conditional statements

```python
# had import re use the function whick i am using to check numbers inputed
import re
# option variable is here allow multiple results to be checked
choice = " "
# option.upper is reduce user error
while str.upper(choice) != "X" :
# checks if inputs are between two points and if not it breaks starts back at
# start of the loop
   print("If you wish to convert Celsius to Fahrenheit press A and if you wish to \nconvert Fahrenheit to Celsius press B\nor X to Quit")

   choice = input("make your choice ")
   choice = str.upper(choice)
   print (choice)

   if choice == "A":
      celsius = input("Enter temperture  you wish to convert to Fahrenheit ")
# checks if varaible match with specified vairables
      match = re.match("^[0-9.]*$", celsius)
      while match == None or celsius == "":
           fahrenheit = input("Please enter Celsius value you wish to convert Fahrenheit ")
           match = re.match("^[0-9.]*$", celsius)
      celsius = float(celsius)

      print(((celsius * 9) / 5) + 32,"°F")
   if choice == "B":
      fahrenheit = input("Enter temperture  you wish to convert to Celsius ")

      match = re.match("^[0-9.]*$", fahrenheit)
      while match == None or fahrenheit == "":
           fahrenheit = input("Please enter Celsius value you wish to convert Fahrenheit ")
           match = re.match("^[0-9.]*$", fahrenheit)
      fahrenheit = float(fahrenheit)


      print(((fahrenheit - 32) * 5) / 9,"°C")
```

If you wish to convert Celsius to Fahrenheit press A and if you wish to 
convert Fahrenheit to Celsius press B
or X to Quit
make your choice A
A
Enter temperture  you wish to convert to Fahrenheit 31
87.8 °F
If you wish to convert Celsius to Fahrenheit press A and if you wish to 
convert Fahrenheit to Celsius press B
or X to Quit
make your choice x
X

---

## 🛣️ Distance Converter
Created a distance conversion application that:

- Converts Miles ➜ Kilometres
- Converts Kilometres ➜ Miles
- Allows the user to perform multiple conversions

## Skills Used
- Loops
- User interaction
- Mathematical calculations

```python
# had import re use the function whick i am using to check numbers inputed
import re
# option variable is here allow multiple results to be checked
choice = " "
# option.upper is reduce user error
while str.upper(choice) != "X" :
# checks if inputs are between two points and if not it breaks starts back at
# start of the loop
   print("If you wish to convert miles to km press A and if you wish to \nconvert km to miles press B.\n or X to Quit")

   choice = input("make your choice ")
   choice = str.upper(choice)
   print (choice)

   if choice == "A":
      miles = input("Enter distance you wish to convert to km ")
# checks if varaible match with specified vairables
      match = re.match("^[0-9.]*$", miles)
      while match == None or miles == "":
           miles = input("Please enter miles value you wish to convert km ")
           match = re.match("^[0-9.]*$", miles)
      miles = float(miles)

      print(miles / 1.60934 ,"km")
   if choice == "B":
      km = input("Enter km  you wish to convert to miles ")
### km=miles×1.60934
      match = re.match("^[0-9.]*$", km)
      while match == None or km == "":
           km = input("Enter km  you wish to convert to miles ")
           match = re.match("^[0-9.]*$", km)
      km = float(km)


      print(km * 1.60934 ,"miles")
```

If you wish to convert miles to km press A and if you wish to 
convert km to miles press B.
 or X to Quit
make your choice a
A
Enter distance you wish to convert to km 56
34.796873252389176 km
If you wish to convert miles to km press A and if you wish to 
convert km to miles press B.
 or X to Quit
make your choice x
X

---

## 🍀 Lucky Number Generator
Designed a fun program that:

- Accepts a 3-digit number
- Separates individual digits
- Calculates the sum of the digits

## Skills Used
- Floor division (`//`)
- Modulus operator (`%`)
- Integer arithmetic

```python
digit = input("Enter a 3-digit number")

digit = int(digit)
hundreds = digit // 100
tens = (digit // 10) % 10
units = digit % 10

print(hundreds + tens + units)
```     
Enter a 3-digit number154
10

---

## 🔐 Secret Code Reverser
Developed a puzzle-solving tool that:

- Accepts a 4-digit number
- Extracts individual digits
- Reverses the number to create a secret code

## Skills Used
- Digit extraction
- Number manipulation
- Mathematical logic

```python
# Step 1: Prompt the user to enter a 4-digit number
number = int(input("Enter a 4-digit number: "))

# Step 2: Separate the digits using floor division (//) and modulus (%)
# Extract the 4th digit (units place)
digit4 = number % 10
# Remove the 4th digit from the number
number = number // 10

# Extract the 3rd digit (tens place)
digit3 = number % 10
# Remove the 3rd digit from the number
number = number // 10

# Extract the 2nd digit (hundreds place)
digit2 = number % 10
# Remove the 2nd digit from the number
number = number // 10

# Extract the 1st digit (thousands place)
digit1 = number % 10

# Step 3: Rebuild the reversed secret code mathematically
secret_code = str(digit4) + str(digit3) + str(digit2) + str(digit1)

# Step 4: Print the secret code
print("The secret code is:", secret_code)
```

Enter a 4-digit number: 3564
The secret code is: 4653

---

# 📅 Day 2 - Decision Making & Loops

## 🔒 Security Door Access System
Created a login system that:

- Checks a user-entered security code
- Grants or denies access
- Locks the account after multiple failed attempts

## Skills Used
- While loops
- Authentication logic
- Conditional statements

```python
password = "4556"
attemps = 0
while attemps < 3:
  user_password = input("Please enter your Bank Pin:")
  if user_password == password:
    print("🔓 Access granted. Welcome inside!")
    break
  else:
    print("⛔ Access denied. Incorrect code.")
    attemps += 1
if attemps == 3:
  print("🔒Account Locked🔒")
```
Enter Password1234
⛔ Access denied. Incorrect code.
Enter Password123
🔓 Access granted. Welcome inside!

---

## 🔢 Divisibility Checker
Built a maths utility that:

- Checks if a number is divisible by both 3 and 7
- Displays clear feedback to the user

## Skills Used
- Modulus operator (`%`)
- Boolean logic

```python
number = int(input("Enter a number: "))
if number % 3 == 0 and number % 7 == 0:
    print(f"{number} is divisible by both 3 and 7.")
else:
    print(f"{number} is not divisible by both 3 and 7.")
```
Enter a number: 21
21 is divisible by both 3 and 7.

---

## 🧮 Menu-Driven Calculator
Developed an interactive calculator capable of:

- Addition
- Subtraction
- Multiplication
- Division
- Exit functionality

## Skills Used
- Menu systems
- Loops
- Conditional statements
- Error handling

```python
option = 0
while option != 5:
  print("1- Addition")
  print("2- Subtraction")
  print("3- Multiplication")
  print("4- Division")
  print("5- Exit")
  option = int(input("Enter option: "))
  if option != 5:
    num1 = int(input("Enter first number: "))
    num2 = int(input("Enter second number: "))
  if option == 1:
    print(f"{num1} + {num2} =",num1 + num2)
  elif option == 2:
    print(f"{num1} - {num2} =",num1 - num2)
  elif option == 3:
    print(f"{num1} * {num2} =",num1 * num2)
  elif option == 4:
    if num2 == 0:
      print("Cannot divide by zero")
    else:
      print(f"{num1} / {num2} =",num1 / num2)
  elif option == 5:
    print("Exit")
  else:
    print("Invalid option")
```
1- Addition
2- Subtraction
3- Multiplication
4- Division
5- Exit
Enter option: 4
Enter first number: 4
Enter second number: 0
Cannot divide by zero
1- Addition
2- Subtraction
3- Multiplication
4- Division
5- Exit
Enter option: 5
Exit

---

## 👟 Fitness Tracker Sum Calculator
Created a program that:

- Calculates the total sum from 1 to a chosen number
- Simulates increasing daily fitness goals

## Skills Used
- For loops
- Accumulators
- Mathematical calculations

```python
day = int(input("Enter a positive number: "))
total = 0
for i in range(1, day + 1):
    total += i
print(f"The sum of numbers from 1 to {day} is {total}")
```

Enter a positive number: 10
The sum of numbers from 1 to 10 is 55

---

## 🔍 Prime Number Checker
Designed a program that:

- Determines whether a number is prime
- Displays an appropriate result

## Skills Used
- Loops
- Decision making
- Number theory

```python
num = int(input("Enter a positive integer: "))
if num == 0 or num == 1:
    print(num, "is not a prime number")
elif num > 1:
    # check for factors
    for i in range(2, num):
        if (num % i) == 0:
            # if factor is found, set flag to True
            flag = True
            # break out of loop
            break

    # check if flag is True
    if flag:
        print(num, "is not a prime number")
    else:
        print(num, "is a prime number")
```

Enter a positive integer: 15
15 is not a prime number

---

## ✖️ Factorial Calculator
Built a factorial calculation tool that:

- Accepts a non-negative integer
- Calculates the factorial value

## Skills Used
- Iteration
- Mathematical problem solving

```python
number = int(input("Enter a non-negative integer: "))
factorial = 1
if number < 0:
    print("Sorry, factorial does not exist for negative numbers")
elif number == 0:
    print("The factorial of 0 is 1")
else:
    for i in range(1, number + 1):
        factorial = factorial * i
    print("The factorial of", number, "is", factorial)
```
Enter a non-negative integer: 5
The factorial of 5 is 120

---

## 📐 Number Pattern Generator
Created a staircase pattern generator using nested loops:


```python
rows = int(input("Enter the number of rows: "))
for i in range(1, rows + 1):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
```
Enter the number of rows: 5
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5 

---

## 🧩 Bonus Challenge: FizzBuzz

One of the most common beginner programming challenges is **FizzBuzz**, which tests the use of loops, conditional statements, and the modulus operator.

## Objective

Create a program that loops through numbers from **1 to 100** and:

- Prints **"Fizz"** if the number is divisible by 3
- Prints **"Buzz"** if the number is divisible by 5
- Prints **"FizzBuzz"** if the number is divisible by both numbers
- Otherwise prints the number itself

## Python Solution

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
