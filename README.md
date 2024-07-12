[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15402731&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.


>Python is a high-level, interpreted programming language known for its simplicity and readability. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming.

Key Features:

-Easy-to-learn: Python's syntax is straightforward and emphasizes readability, making it accessible for beginners.
-Extensive Libraries: Python has a vast standard library and numerous third-party libraries for various tasks.
-Versatility: It's used for web development, data analysis, artificial intelligence, scientific computing, automation, and more.

Example Use Cases:

-Web Development (Django, Flask)
-Data Science and Machine Learning (NumPy, Pandas, TensorFlow)
-Automation (Scripting, Web Scraping)
-Scientific Computing (SciPy)


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.


Steps to Install Python:

Windows:

-Download Python installer from python.org.
-Run the installer and follow on-screen instructions.
-Ensure to check "Add Python to PATH" during installation on Windows.

Verify Installation:

-Open a terminal or command prompt.
-Type python --version to check Python version.
-Type python to enter the Python interpreter.

Setting up Virtual Environment:

-Install virtualenv via pip (pip install virtualenv).
-Create a virtual environment: virtualenv myenv.

Activate the virtual environment:
     Windows: myenv\Scripts\activate




3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.


Python program
   
      print("Hello, World!")

Explanation
    -print: This is a built-in function that displays the message inside the parentheses onto the console.
   -"Hello, World!": This is a string literal enclosed in double quotes, representing the text to be printed.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.


-Integers: Whole numbers (e.g., 10, -5).
-Floats: Numbers with decimal points (e.g., 3.14, -1.23).
-Strings: Sequences of characters (e.g., "Hello", 'World!').
-Booleans: True or False values.

> an example of a python program demonstrating variables of different data types
age = 25        # Integer
pi = 3.14159     # Float
name = "Alice"    # String
is_valid = True   # Boolean

print("Age:", age)
print("Pi:", pi)
print("Name:", name)
print("Valid", is_valid)




5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

-Conditional statements (if-else): These statements control program flow based on certain conditions.

-an example program
    age = 18

   if age >= 18:
    print("You are eligible to vote.")
    else:
    print("Sorry, you are not eligible to vote.")

Loops (for loop): Loops allow for repeated execution of a block of code a certain number of times.

a for loop program
          for i in range(1, 5):
          print(i)




6. Functions in Python:

   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

*Functions are reusable blocks of code that perform specific tasks. They take arguments (optional inputs) and can return a value.


example of a function  program :-                          
     def sum_two_numbers(a, b):
        return a + b


     result = sum_two_numbers(3, 5)
     print("Sum:", result) 



7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

-Lists: Ordered collection of items ([1, 2, 3]), accessed by index.
-Dictionaries: Unordered collection of key-value pairs ({"name": "Alice", "age": 30}), accessed by keys.

example program:-
       numbers = [1, 2, 3, 4, 5]


       person = {"name": "John", "age": 30}
          print(numbers[0])     
       print(person["name"])   





8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.


Exception Handling-Handles errors gracefully to prevent program crashes.

 python pprogram showing how to use exception handling

      try:
           result = 10 / 0
     except ZeroDivisionError:
           print("Error: Division by zero!")
     finally:
          print("Execution completed.")





9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

-Module: A file containing Python definitions and statements.
-Package: A directory containing modules and an __init__.py file.

  Importing and Using Modules example:-
        import math

         print(math.sqrt(16))  






10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

   Reading from a File:

 Open the file: Use the open() function with the desired filename and access mode ('r' for reading).

Read the content:

-read(): Reads the entire file content as a string.
-readline(): Reads a single line from the file.
-readlines(): Reads all lines from the file and stores them in a list.
-Close the file: Use the close() method on the file object to release resources.

Example Script (Read a File):
       def read_file(filename):
  
        try:
          with open(filename, 'r') as file:
          content = file.read()
          print(content)
       except FileNotFoundError:
           print(f"Error: File '{filename}' not found.")

   # Example usage
          read_file("my_file.txt")


          Writing to a File:

-Open the file: Use the open() function with the desired filename and access mode ('w' for writing or 'a' for appending).

-Write data: Use the write() method on the file object to write content (strings or lists of strings with conversion).

-Close the file: Similar to reading, use close() to release resources.

    Example Script (Write to a File):

       def write_to_file(filename, data):
 
         try:
            with open(filename, 'w') as file:
           for item in data:
             file.write(item + "\n") 
        except Exception as e:  
            print(f"Error writing to file: {e}")

   # Example usage
       data = ["Line 1", "Line 2", "Line 3"]
        write_to_file("my_data.txt", data)






# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


