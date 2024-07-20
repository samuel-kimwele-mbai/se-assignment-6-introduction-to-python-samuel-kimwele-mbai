[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15438064&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   - Python is a high-level, interpreted programming language known for its simplicity and readability. Key features include dynamic typing, extensive standard library, portability, and support for object-oriented programming. Use cases include web development (Django, Flask), data science (pandas, NumPy), automation, and scripting.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   - Download Python: Go to the Python website and download the latest version.
- Run the Installer: Execute the downloaded installer and check "Add Python to PATH".
- Customize Installation: Choose "Customize installation" and ensure "pip" and "IDLE" are selected.
- Finish Installation: Complete the installation process.
- Verify Installation:

- Open Command Prompt and type python --version.
- Verify pip installation with pip --version.
- Set Up Virtual Environment:

- Open Command Prompt.
- Install virtualenv: pip install virtualenv.
- Create a virtual environment: virtualenv venv.
- Activate the environment: .\venv\Scripts\activate.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   - print("Hello, World!")
   - print(): This is a built-in function in Python that outputs the specified message to the console. Functions in Python are called using parentheses.

"Hello, World!": This is a string literal enclosed in double quotes. Strings in Python can be enclosed in either single quotes (') or double quotes (").

- Breakdown
- Function Call: print() is a function call. Functions are blocks of code that perform a specific task.
- String Literal: "Hello, World!" is the argument passed to the print() function. It's the text to be printed.
- Parentheses: Parentheses () are used to enclose the arguments passed to a function.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   - Integer (int): Whole numbers, positive or negative, without decimals.
Example: 5, -42
- Float (float): Numbers, positive or negative, containing one or more decimals.
Example: 3.14, -0.001
- String (str): A sequence of characters enclosed in quotes (single, double, or triple).
Example: 'hello', "world"
- Boolean (bool): Represents one of two values: True or False.
Example: True, False
- List (list): An ordered collection of items which can be of different types.
Example: [1, 2, 3], ['apple', 'banana']
- Tuple (tuple): An ordered collection of items, similar to a list, but immutable.
Example: (1, 2, 3), ('apple', 'banana')
- Dictionary (dict): A collection of key-value pairs.
Example: {'name': 'Alice', 'age': 25}
- Set (set): An unordered collection of unique items.
Example: {1, 2, 3}, {'apple', 'banana'}
- Script Demonstrating Different Data Types
- # Integer
age = 30
print("Age:", age)  # Output: Age: 30

# Float
height = 5.9
print("Height:", height)  # Output: Height: 5.9

# String
name = "Alice"
print("Name:", name)  # Output: Name: Alice

# Boolean
is_student = True
print("Is student:", is_student)  # Output: Is student: True

# List
fruits = ["apple", "banana", "cherry"]
print("Fruits:", fruits)  # Output: Fruits: ['apple', 'banana', 'cherry']

# Tuple
coordinates = (10.0, 20.0)
print("Coordinates:", coordinates)  # Output: Coordinates: (10.0, 20.0)

# Dictionary
person = {"name": "Alice", "age": 30}
print("Person:", person)  # Output: Person: {'name': 'Alice', 'age': 30}

# Set
unique_numbers = {1, 2, 3, 2, 1}
print("Unique numbers:", unique_numbers)  # Output: Unique numbers: {1, 2, 3}


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   - Conditional statements in Python allow you to execute different blocks of code based on certain conditions. The most common conditional statement is the if-else statement.

- if-else Statement Example
- # Conditional statement example
age = 18

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
- Loops
Loops in Python are used to repeatedly execute a block of code. The two main types of loops are for loops and while loops.

for Loop Example
# For loop example
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   - Functions in Python are blocks of reusable code that perform a specific task. They help in organizing code, reducing redundancy, and improving readability. Functions can take arguments, process them, and return a result.
   - # Define a function that takes two arguments and returns their sum
def add_numbers(a, b):
    return a + b

# Call the function with example arguments
result = add_numbers(3, 5)
print("The sum is:", result)  # Output: The sum is: 8



7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   - Lists:

- Ordered collections of items.
- Indexed by integers starting from 0.
- Allow duplicate elements.
- Syntax: [].
- Dictionaries:

- Unordered collections of key-value pairs.
- Indexed by unique keys, which can be of any immutable type.
- Do not allow duplicate keys.
- Syntax: {}.

- Script Demonstrating Lists and Dictionaries
- # Creating a list of numbers
numbers = [1, 2, 3, 4, 5]

# Basic operations on a list
print("Original list:", numbers)           # Output: [1, 2, 3, 4, 5]
numbers.append(6)
print("List after appending 6:", numbers)  # Output: [1, 2, 3, 4, 5, 6]
numbers.remove(3)
print("List after removing 3:", numbers)   # Output: [1, 2, 4, 5, 6]
print("Second element:", numbers[1])       # Output: 2
print("Length of the list:", len(numbers)) # Output: 5

# Creating a dictionary with key-value pairs
person = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
}

# Basic operations on a dictionary
print("Original dictionary:", person)           # Output: {'name': 'Alice', 'age': 30, 'city': 'New York'}
person["email"] = "alice@example.com"
print("Dictionary after adding email:", person) # Output: {'name': 'Alice', 'age': 30, 'city': 'New York', 'email': 'alice@example.com'}
del person["age"]
print("Dictionary after deleting age:", person) # Output: {'name': 'Alice', 'city': 'New York', 'email': 'alice@example.com'}
print("Name:", person["name"])                  # Output: Alice
print("Keys in the dictionary:", list(person.keys()))   # Output: ['name', 'city', 'email']
print("Values in the dictionary:", list(person.values())) # Output: ['Alice', 'New York', 'alice@example.com']


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   - Exception handling in Python allows you to manage and respond to runtime errors in a controlled manner. By using try, except, and finally blocks, you can catch exceptions, handle them, and execute cleanup actions regardless of whether an error occurred.

- Example of Exception Handling
- def divide(a, b):
    try:
        result = a / b
    except ZeroDivisionError:
        print("Error: Division by zero is not allowed.")
        result = None
    except TypeError:
        print("Error: Both arguments must be numbers.")
        result = None
    else:
        print("Division successful.")
    finally:
        print("Execution of try-except block completed.")
    return result



9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   - Modules: A module is a single Python file that contains definitions and statements. Modules help in organizing code into manageable sections. They can contain functions, classes, and variables. Modules are imported into other Python scripts to use the functions, classes, and variables defined within them.

- Packages: A package is a collection of related modules organized in a directory hierarchy. Each directory contains an __init__.py file (which can be empty) to signify that the directory is a package. Packages help in organizing and distributing modules in a structured way.
- # Import the math module
import math

# Use functions from the math module
print("Value of pi:", math.pi)           # Output: Value of pi: 3.141592653589793
print("Square root of 16:", math.sqrt(16)) # Output: Square root of 16: 4.0
print("Factorial of 5:", math.factorial(5)) # Output: Factorial of 5: 120

# Using a specific function from the math module
from math import pow

# Calculate 2 raised to the power of 3
print("2 to the power of 3:", pow(2, 3)) # Output: 2 to the power of 3: 8.0


- Importing the Module:

import math: Imports the entire math module, allowing access to its functions and constants using the math. prefix.
- Using Functions and Constants:

math.pi: Accesses the constant pi from the math module.
math.sqrt(16): Calls the sqrt function to compute the square root of 16.
math.factorial(5): Calls the factorial function to compute the factorial of 5.
- Importing Specific Functions:

from math import pow: Imports the pow function directly from the math module, allowing you to use it without the math. prefix.
pow(2, 3): Computes 2 raised to the power of 3 using the pow function.

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    - File I/O (Input/Output) in Python allows you to read from and write to files using built-in functions. You generally use open() to open a file and then read or write data using file methods. Always remember to close the file after performing operations or use a with statement to handle it automatically.
    - Reading from a File
Here is a script that reads the content of a file and prints it to the console:
# Reading from a file
file_path = 'example.txt'

try:
    with open(file_path, 'r') as file:
        content = file.read()
        print("File content:")
        print(content)
except FileNotFoundError:
    print(f"Error: The file '{file_path}' does not exist.")
except IOError:
    print("Error: An I/O error occurred.")

- Writing to a File
Here is a script that writes a list of strings to a file:
# Writing to a file
file_path = 'output.txt'
lines = ["Hello, World!", "This is a test file.", "Python file I/O is easy!"]

try:
    with open(file_path, 'w') as file:
        for line in lines:
            file.write(line + '\n')
    print(f"Data successfully written to '{file_path}'.")
except IOError:
    print("Error: An I/O error occurred.")


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


