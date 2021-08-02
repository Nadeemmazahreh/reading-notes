## What is a variable scope? 
    The concept of scope rules how variables and names are looked up in your code. It determines the visibility of a variable within the code. The scope of a name or variable depends on the place in your code where you create that variable. The Python scope concept is generally presented using a rule known as the LEGB rule.

## There are 2 general Scopes
    1-  Global scope: The names that you define in this scope are available to all your code. 

    2-  Local scope: The names that you define in this scope are only available or visible to the code within the scope. 

## LEGB Rule 
    1-   Local (or function) scope is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function.

    2-  Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function.

    3-  Global (or module) scope is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

    4-  Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python.

## Class and Instance Attributes Scope
    When you define a class, you’re creating a new local Python scope. The names assigned at the top level of the class live in this local scope. The names that you assigned inside a class statement don’t clash with names elsewhere.



