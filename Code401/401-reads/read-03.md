## What is a file? 
    a file is a contiguous set of bytes used to store data

    Parts of a file 
        - Header: metadata about the contents of the file (file name, size, type, and so on) 
        - Data: contents of the file as written by the creator or editor 
        - End of file (EOF): special character that indicates the end of the file 

## What is a file path
    When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file

## Opening and Closing a File in Python
    to open a file use open() function

## Exceptions versus Syntax Errors
    Syntax errors occur when the parser detects an incorrect statement. Ecexption error occurs whenever syntactically correct Python code results in an error.

## Raising an Exception
    Use raise to force and exeption
    Example: 
        x = 10
        if x > 5:
        raise Exception('x should not exceed 5. The value of x was: {}'.format(x))  
## The AssertionError Exception
    Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

## The try and except Block: Handling Exceptions
    The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

## Else Exeption
    else lets you code sections that should run only when no exceptions are encountered in the try clause.

## Finally Exeption
    finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.
