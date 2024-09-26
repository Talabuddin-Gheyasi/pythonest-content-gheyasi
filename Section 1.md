# PCEP-30-02 1.1: Understand Fundamental Terms and Definitions

## Interpreting and the Interpreter
**1. Interpreter**: An interpreter is a program that executes other programs directly, translating high-level programming languages into machine code line-by-line at runtime. This allows for easier debugging and immediate execution of code.

**Example:** Python uses an interpreter, allowing you to run code interactively:

'''python title="Example"
print("Hello, World!")
'''

## 2. Compilation and the Compiler
Compiler: A compiler translates the entire source code of a program into machine code before execution. This process usually results in faster execution because the code is precompiled.

**Example:** C/C++ uses compilers. For instance, if you have a C program:
'''python title="Example"
#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}
'''

## 3. Lexis ##
Lexis: This refers to the vocabulary of a programming language, including keywords, operators, and identifiers. Lexical elements include identifiers like variable names and reserved keywords.

**Example:** In Python, keywords include if, else, def, etc.

## 4. Syntax ##
Syntax: The rules that define the structure of statements in a programming language. Syntax errors occur when code violates these rules.

**Example:** In Python, a function definition must include a colon:
'''python title="Example"
def my_function():  # Correct syntax
    pass
'''
## 5. Semantics ##
Semantics: The meaning of the statements in a programming language. While syntax defines the structure, semantics defines the behavior of the code.

**Example:** The statement x = 5 assigns the integer value 5 to the variable x. The semantics explains what happens during execution.

**Questions:**

Multiple Choice: What is the main function of an interpreter?

A) To execute the program line-by-line
B) To compile the entire program before execution
C) To identify syntax errors
D) To convert machine code to high-level code
Answer: A) To execute the program line-by-line

True/False: A compiler can detect runtime errors before the program is executed.

Answer: False (compilers can detect syntax errors but not runtime errors).

Code Compilation: What type of error does the following code produce?

'''python title="Example"
if (x > 10)
    print("x is greater than 10")
'''
**Answer:** SyntaxError (missing colon after if statement).

**Multiple Choice:** Which of the following terms refers to the meaning of a programming statement?

A) Syntax
B) Lexis
C) Semantics
D) Compilation
**Answer:** C) Semantics

True/False: Lexis includes the set of valid identifiers in a programming language.

Answer: True

Code Compilation: Identify the error in this code snippet:

'''python title="Example"
def example_function()
    print("Hello!")
'''
**Answer:** SyntaxError (missing colon after function definition).

**Multiple Choice:** In which of the following languages is the term "interpreter" most commonly used?
A) C++
B) Java
C) Python
D) Assembly
**Answer:** C) Python

**True/False:** Syntax errors prevent a program from running until they are fixed.

**Answer:** True

**Code Compilation:** Given the following code, what type of error will it generate?
'''python title="Example"
for i in range(5)
    print(i)

'''
**Answer:** SyntaxError (missing colon after for statement).

**Multiple Choice:** What is the output of the following code if executed successfully?
'''python title="Example"
def my_func():
    return 3 + 5
print(my_func())
'''
A) 3 + 5
B) 8
C) my_func
D) None
**Answer:** B) 8


# PCEP-30-02 1.2: Understand Python’s Logic and Structure #
## 1. Keywords ##
**Definition:**
Keywords are reserved words in Python that have special meaning. They cannot be used as identifiers (such as variable names) because they are integral to the syntax and functionality of the language.

**Examples:**
if, else, elif: Used for conditional statements.
for, while: Used for loops.
def: Used to define a function.
import: Used to include modules.

'''python title="Example"
Copy code
def check_even(number):
    if number % 2 == 0:
        return True
    else:
        return False

print(check_even(10))  # Output: True
'''

**Questions:**
Multiple Choice: Which of the following is a Python keyword?

A) variable
B) for
C) function
D) define
**Answer:** B) for

**True/False:** The keyword import is used to define a function in Python.

**Answer:** False

Code Compilation: What error will this code produce?

'''python title="Example"
def = 5
**Answer:** SyntaxError (invalid syntax).

**Multiple Choice:** How many keywords are there in Python 3.x?

A) 30
B) 35
C) 50
D) 25
**Answer:** B) 35

**True/False:** You can use a keyword as a variable name in Python.

**Answer:** False

**Code Compilation:** What is the output of the following code?

'''python title="Example"
if True:
    print("True")
'''
**Answer:** True

Multiple Choice: Which keyword is used to define a function in Python?

A) func
B) define
C) def
D) function
Answer: C) def

True/False: The keyword elif is short for "else if".

Answer: True

Code Compilation: What is the output of this code?

python
Copy code
print(type('Hello World'))
Answer: <class 'str'>

Multiple Choice: Which of the following is NOT a keyword in Python?

A) None
B) return
C) print
D) import
Answer: C) print

2. Instructions
Definition:
Instructions are commands that tell the Python interpreter what to do. They can perform actions such as calculations, data manipulation, and control flow.

Examples:

Assignment: x = 10
Function call: print("Hello")
Control flow: if, for, while statements.
Example Code:

python
Copy code
number = 5
if number > 0:
    print("Positive")
else:
    print("Negative or Zero")
Questions:

Multiple Choice: Which of the following is an example of an instruction in Python?

A) if x > 10:
B) x = 5
C) print("Hello")
D) All of the above
Answer: D) All of the above

True/False: An instruction in Python cannot change the value of a variable.

Answer: False

Code Compilation: What will this code output?

python
Copy code
x = 5
print(x * 2)
Answer: 10

Multiple Choice: Which of the following instructions will cause an error?

A) y = 10
B) print(y)
C) y + 5
D) z = y
Answer: C) y + 5 (it doesn't assign the result).

True/False: The instruction print() will output text to the console.

Answer: True

Code Compilation: What error does the following code produce?

python
Copy code
print(5 + )
Answer: SyntaxError (invalid syntax).

Multiple Choice: What does the instruction x += 1 do?

A) Increments x by 1
B) Decreases x by 1
C) Resets x to 1
D) None of the above
Answer: A) Increments x by 1

True/False: You can have multiple instructions on one line in Python by separating them with a semicolon.

Answer: True

Code Compilation: What is the result of executing the following code?

python
Copy code
a = 2
b = 3
print(a + b)
Answer: 5

Multiple Choice: Which instruction is used to get user input?

A) input()
B) scan()
C) read()
D) get()
Answer: A) input()

3. Indentation
Definition:
Indentation is the whitespace at the beginning of a line that determines the structure and grouping of code blocks in Python. Unlike many languages that use braces, Python uses indentation to define code blocks.

Examples:

Indentation is required after control statements like if, for, and while.
Example Code:

python
Copy code
for i in range(3):
    print(i)  # This line is indented, indicating it is part of the loop.
Questions:

Multiple Choice: Why is indentation important in Python?

A) It is purely aesthetic.
B) It defines the scope of code blocks.
C) It is not required.
D) It makes the code run faster.
Answer: B) It defines the scope of code blocks.

True/False: Indentation can be done using both spaces and tabs interchangeably in Python.

Answer: False

Code Compilation: What error does this code produce?

python
Copy code
if True:
print("True")
Answer: IndentationError

Multiple Choice: How many spaces are typically used for indentation in Python?

A) 1
B) 2
C) 4
D) 8
Answer: C) 4

True/False: Indentation is optional in Python.

Answer: False

Code Compilation: What is the output of the following code?

python
Copy code
if True:
    print("Hello")
else:
    print("World")
Answer: Hello

Multiple Choice: What happens if the indentation level is inconsistent in a code block?

A) The code will execute normally.
B) It will raise an IndentationError.
C) The code will run, but with unexpected results.
D) It will produce a syntax error.
Answer: B) It will raise an IndentationError.

True/False: You can use different numbers of spaces for indentation in different blocks of code.

Answer: True (but it may lead to errors if not consistent).

Code Compilation: What will this code output?

python
Copy code
def my_function():
    print("Start")
    print("End")

my_function()
Answer:

sql
Copy code
Start
End
Multiple Choice: Which of the following is a correct indentation practice in Python?

A) Using both tabs and spaces in the same block
B) Consistently using 4 spaces for all indents
C) Using varying spaces for different lines
D) Not using any indentation
Answer: B) Consistently using 4 spaces for all indents

4. Comments
Definition:
Comments are annotations in the code that are not executed by the interpreter. They are used to explain the code, making it easier to understand.

Examples:

Single-line comments start with #.
Multi-line comments can be enclosed in triple quotes (""" or ''').
Example Code:

python
Copy code
# This is a single-line comment
def my_function():
    """This function prints a message."""
    print("Hello, World!")

my_function()
Questions:

Multiple Choice: Which symbol is used for single-line comments in Python?

A) //
B) --
C) #
D) /*
Answer: C) #

True/False: Comments are executed by the Python interpreter.

Answer: False

Code Compilation: What will the following code output?

python
Copy code
print("This will run")  # This comment will be ignored
Answer: This will run

Multiple Choice: How can you create a multi-line comment in Python?

A) Using //
B) Using # on each line
C) Using """ or '''
D) Using /* ... */
Answer: C) Using """ or '''

True/False: Comments can help improve code readability.

Answer: True

Code Compilation: What is the output of the following code?

python
Copy code
def example():
    """This function does nothing."""
    pass

print(example())
Answer: None

Multiple Choice: What will happen if you forget to add a comment symbol (#) at the beginning of a line meant to be a comment?

A) The line will execute as code.
B) It will cause a syntax error.
C) It will be ignored by the interpreter.
D) It will create a runtime error.
Answer: A) The line will execute as code.

True/False: You can use comments to temporarily disable code.

Answer: True

Code Compilation: Which line below is a correct comment?

python
Copy code
# This is a comment
print("Hello")  # Print a greeting
Answer: Both lines are correct comments.

Multiple Choice: Which of the following is NOT a reason to use comments in code?

A) To explain complex logic
B) To improve readability
C) To make code run faster
D) To provide context for future changes
Answer: C) To make code run faster

Summary
In this section, we explored Python’s logic and structure, focusing on:

Keywords: Reserved words that define the syntax and functionality.
Instructions: Commands that direct the interpreter to perform actions.
Indentation: The whitespace that defines code blocks and structure.
Comments: Non-executable lines that help explain and annotate code.
