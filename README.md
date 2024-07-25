[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15466521&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
  
Python is a high-level, interpreted programming language known for its simplicity and readability. 
 Python's syntax is clean and easy to understand, making it accessible to beginners and allowing developers to write and maintain code efficiently.
 Python is executed line by line, which makes debugging easier and more interactive.
 Python runs on various platforms, including Windows, macOS, Linux, and more, making it a versatile choice for development.






2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.



Download Python Installer: Go to the official Python website and download the latest Python installer for Windows.
Run Installer: Run the downloaded installer. Check the box "Add Python to PATH" and select "Install Now".

Verify Installation: 
Open Command Prompt and run:
python --version

> Setting Up a Virtual Environment
Install venv (if not already available) by running the following code:

python3 -m ensurepip --upgrade

Create Virtual Environment:
python3 -m venv myenv

This creates a directory named myenv containing the virtual environment.

Activate Virtual Environment:

Windows:
myenv\Scripts\activate





3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")

print Function:
print is a built-in function in Python used to output text or other values to the console.

Quotation Marks ("):
The quotation marks (" ") enclose the string "Hello, World!".
In Python, strings can be defined using either single quotes (' ') or double quotes (" "). They are interchangeable unless the string itself contains a quote character.

Parentheses (()):
The parentheses are used to pass arguments to the function. In this case, "Hello, World!" is the argument passed to the print function.

String:
A string in Python is a sequence of characters. In this example, "Hello, World!" is a string literal, meaning the value of the string is explicitly written in the code.




4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.


BASIC DATA TYPES IN PYTHON
Integers (int): Whole numbers, positive or negative, without decimals. Example: 5, -3.

Floating-point numbers (float): Numbers with decimal points. Example: 3.14, -0.001.

Strings (str): A sequence of characters enclosed in single or double quotes. Example: "hello", 'world'.

Booleans (bool): Represents one of two values: True or False.

Lists (list): An ordered collection of items, which can be of different types. Lists are mutable. Example: [1, 2, 3], ["apple", "banana"].

Tuples (tuple): An ordered collection of items similar to lists, but tuples are immutable. Example: (1, 2, 3), ("apple", "banana").

Dictionaries (dict): A collection of key-value pairs. Example: {"name": "John", "age": 30}.

Sets (set): An unordered collection of unique items. Example: {1, 2, 3}, {"apple", "banana"}.

Script Demonstrating Variables of Different Data Types

# Integer
age = 25
print("Age:", age)

# Float
pi = 3.14159
print("Pi:", pi)

# String
greeting = "Hello, World!"
print("Greeting:", greeting)

# Boolean
is_student = True
print("Is Student:", is_student)

# List
fruits = ["apple", "banana", "cherry"]
print("Fruits:", fruits)

# Tuple
coordinates = (10.5, 20.3)
print("Coordinates:", coordinates)

# Dictionary
person = {"name": "Alice", "age": 30}
print("Person:", person)

# Set
unique_numbers = {1, 2, 3, 4, 5}
print("Unique Numbers:", unique_numbers)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

Conditional statements allow you to execute different blocks of code based on certain conditions. The most common conditional statements in Python are if, elif, and else.

if-else Statement Example


age = 18

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions are reusable blocks of code that perform a specific task. They allow you to encapsulate logic, making your code more modular, organized, and easier to maintain. Functions can take inputs, known as arguments, and can return outputs

BENEFITS OF USING FUNCTIONS
Modularity: Breaks down complex problems into smaller, manageable pieces.

Reusability: Once defined, functions can be reused across different parts of the program or in different projects.

Readability: Functions with descriptive names can make code easier to read and understand.

Maintainability: Easier to update or debug parts of the code without affecting the whole program.

Example: A Function to Sum Two Numbers

def add_numbers(a, b):
    """
    This function takes two arguments and returns their sum.
    """
    return a + b

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.


Differences Between Lists and Dictionaries in Python

Lists:

Ordered collections of items.
Indexed by integers, starting from 0.
Items can be of any data type and can be repeated.
Syntax: Defined using square brackets, e.g., my_list = [1, 2, 3].

Dictionaries:

Unordered collections of key-value pairs.
Keys must be unique and immutable (e.g., strings, numbers, tuples), while values can be of any type and can be repeated.
Syntax: Defined using curly braces, e.g., my_dict = {"key1": "value1", "key2": "value2"}.

# Creating a list of numbers
numbers = [1, 2, 3, 4, 5]
numbers.append(6)  # Adding an element
numbers.remove(3)  # Removing an element
print("List:", numbers)

# Creating a dictionary with key-value pairs
person = {"name": "John", "age": 25, "city": "New York"}
person["occupation"] = "Developer"  # Adding a key-value pair
person["age"] = 26  # Updating an existing value
del person["city"]  # Removing a key-value pair
print("Dictionary:", person)






8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling in Python is a mechanism to handle runtime errors, allowing a program to continue running or gracefully exit. This is achieved using try, except, and finally blocks, which let you manage exceptions (errors) that may occur during execution.

def divide_numbers(a, b):
    try:
        # Attempt to divide two numbers
        result = a / b
    except ZeroDivisionError:
        # Handle division by zero error
        print("Error: Cannot divide by zero.")
        result = None
    except TypeError:
        # Handle incorrect data type error
        print("Error: Invalid input type. Please provide numbers.")
        result = None
    else:
        # Executed if no exception was raised
        print("Division successful.")
    finally:
        # Executed regardless of an exception occurring
        print("Execution complete.")
    return result

# Example usage
print(divide_numbers(10, 2))  # Should print 5.0 and a success message
print(divide_numbers(10, 0))  # Should handle division by zero
print(divide_numbers(10, 'a'))  # Should handle type error




9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
  
A module is a single file containing Python definitions and statements, such as functions, classes, and variables. It allows you to organize and reuse code across different scripts.
Modules can be imported into other scripts using the import statement.

A package is a collection of related modules grouped together in a directory. Packages allow you to organize modules hierarchically.
A package directory must contain a special file named __init__.py (which can be empty) to be recognized as a package by Python.




Example Using the math Module

import math

# Using functions from the math module
square_root = math.sqrt(16)  # Computes the square root of 16
pi_value = math.pi           # Accesses the value of pi

print("Square root of 16:", square_root)
print("Value of pi:", pi_value)



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from a File: Use open() in read mode ('r') and the read() method to get the file's contents.

Writing to a File: Use open() in write mode ('w') and the write() method to save data to the file.

Script to Read from a File

# Reading from a file
with open('example.txt', 'r') as file:
    content = file.read()
    print("File content:")
    print(content)

Script to Write to a File

# Writing to a file
lines = ["Hello, World!", "Welcome to Python file I/O.", "This is the third line."]

with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + '\n')



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


