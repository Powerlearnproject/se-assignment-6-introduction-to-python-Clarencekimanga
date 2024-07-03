[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15343828&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:
  
1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective. 
   PYTHON IS A HIGH LEVEL PROGRAMMING LANGUAGE, DESIGNED TO BE MORE HUMAN READABLE. IT IS A POPULAR AMONG DEVELOPERS DUE TO ITS: (I) READABILITY. (II) PORTABILITY. (III) ABSTRACTION. (IV) AUTOMICITY IN MEMORY MANAGEMENT. USE CASES INCLUDE: (I) WEB DEVELOPMENT. (II) PROTOTYPING. (III) SOFTWARE DEVELOPMENT. (IV) DATA HANDLING. 

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   (I) VISIT THE PYTHON.ORG SITE.
   (II) UNDER THE DOWNLOADS SECTION, CHOOSE THE LATEST STABLE VERSION.
   (III) ONCE THE DOWNLOAD IS COMPLETE, CLICK INSTALL; HOWEVER, MAKE SURE THAT YOU'VE ADDED IT TO THE SYSTEM PATH.
   (IV) ONCE THE INSTALLATION IS COMPLETE, VERIFY PYTHON VERSION INSTALLED BY RUNNING THE FOLLOWING COMMAND "python --version" IN GIT BASH TERMIMAL.

   SETTING UP A VIRTUAL ENVIRONMENT. 
   (I) CD TO YOUR WORKING FOLDER. 
   (II) RUN THE COMMAND "python -m venv <environment_name>"
   (III) TO ACTIVATE THE ENVIRONMENT RUN THE COMMAND "source ./<environment_name>/Scripts/activate

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   A BASIC PYTHON PROGRAM THAT PRINTS HELLO WORLD TO THE CONSOLE.
   print("Hello, World")
   
   BASIC SYNTAX USED.
   (I) FUNCTION print()
   (II) STRING LITERAL "Hello, World"

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   (I) INTEGER DATA TYPES-REPRESENTS WHOLE NUMBERS
   (II) STRING- RERESENTS TEXTUAL DATA.
   (III) FLOAT- REPRESENTS DECIMAL NUMBERS.
   (IV) COMPLEX- REPRESENTS COMPLEX NUMBERS.
   (V) BOOLEANS- REPRESENTS TRUE OR FALSE VALUES. 
   (VI) BYTES- STORE BINARY DATA. 
   A SCRIPT TO DEMONSTRATE THE CREATION AND USE OF VARIABLES OF DIFFERENT DATA TYPES. 
 # integer.
 x= 5
print("x",x)
# string
name= "clarence"
print("name", name)
# float
area= 50.5
print("area", area)
# boolean
is_student = true
print("student", is_student) 

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   CONDITIONAL STATEMENTS AND LOOPS ARE USED TO ITERATE OVER A GIVEN A INSTRUCTION UNTIL A CERTAIN CONDITON IS MET.
  # if-else statement
age = 35
if age <= 35:
    print("Youth")
else:
    print("Adult")

# Loop through numbers from 1 to 9
for i in range(1, 10):
    print(i, end="")

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   A FUNCTION IS A REUSABLE NAMED BLOCK OF CODE THAT PERFORMS A SPECIFIC TASK OR RETURNS A VALUE. 

   A PROGRAM TO CALCULATE THE SUM OF TWO NUMBERS.
   # custom function to add two numbers
def sum(a,b):
    return a + b
   # usage
    a= 5
    b= 5
    result =sum(a,b)
    print(f"the sum is: {result}")

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   LISTS ARE PART OF THE SEQUENTIAL DATA TYPES, AND REPRESENTS ORDERED COLLECTION OF ITEMS. WHILE DICTIONARIES BELONG THE MAPPING DATA TYPES, AND REPRESENT KEY-VALUE PAIRS. 

A SCRIPT THAT CREATES A LIST OF NUMBERS.
N = 10
numbers = [i for i in range(1, N + 1)]
print(numbers)

A SCRIPTS THAT CREATES A DICTIONARY WITH SOME KEY-VALUES
# creating a dictonary 
country_capitals = {
   "Kenya": "Nairobi",
   "Nigeria": "Lagos",
   "USA": "Washington DC"
}
# accessing values using keys
print(country_capitals["Kenya"])
print(country_capitals["Nigeria"])

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   EXEMPTION HANDLING ALLOWS ONE TO HANDLE ERRORS AND UNEXPECTED SITUATIONS THAT MAY OCCUR DURING A PROGRAM EXECUTION. 
   (I) TRY- CONTAINS THE CODE THAT MAY CONTAIN AN EXEPTION.
   (II) EXCEPT- IF AN EXCEPTION OCCURS THE PROGRAM JUMPS TO THE CORRESPONDING EXCEPT BLOCK.
   (III) FINALLY- IT ENSURES THAT A CERTAIN CODE RUNS EVEN IF AN EXECEPTION IS RAISED OR NOT. 
   # TRY-EXCEPT 
   try:
    numerator = 10
    denominator = 0
    result = numerator / denominator
    print("Result:", result)
except ZeroDivisionError:
    print("Error: Division by zero")

# FINALLY
def read_file(filename):
    try:
        file = open(filename, "r")
        content = file.read()
    except FileNotFoundError:
        print(f"File '{filename}' not found.")
    else:
        print(f"File content: {content}")
    finally:
        file.close()  # Always close the file, even if an exception occurred

# Example usage
read_file("mydata.txt")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
A MODULE IS SELF CONTAINED UNIT THAT CONTAINS A PYTHON CODE. WHILE PACKAGES ARE DIRECTORIES THAT CONTAIN ONE OR MORE RELATED PYTHON MODULES. 
# importing and using the math module 

print(math.sqrt(100))

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
TO READ FROM A FILE, USE THE read() METHOD. EXAMPLE
# reading from file
file_path = "#.txt"
with open(file_path, "r") as file:
content = file.read()
print(content)

TO WRITE TO A FILE USE THE write() METHOD.
# writing to a file
file_path = "#.txt"
with open(file_path, "w") as file:
file.write("greetings\n")
file.write("this is a new line.")

