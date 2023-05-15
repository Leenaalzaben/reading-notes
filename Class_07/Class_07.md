# Variable Scope in Python

Variable scope in Python refers to the region or context in which a variable is defined and can be accessed. It determines the visibility and lifetime of a variable within a program. Python has two main types of variable scope: local scope and global scope.

## Local Scope

Variables defined within a function or block of code have a local scope. They are accessible only within that specific function or block. Local variables are created when the function or block is executed and destroyed when it completes. Other functions or blocks cannot access these variables.

```python
def my_function():
    x = 10  # Local variable
    print("Inside the function:", x)

my_function()
print("Outside the function:", x)  # Raises an error
```

# Global Scope

Variables defined outside any function or block of code have a global scope. They are accessible from anywhere within the program, including inside functions

```python
x = 10  # Global variable

def my_function():
    print("Inside the function:", x)

my_function()
print("Outside the function:", x)
```

# Global and Nonlocal Keywords in Python

In Python, the `global` and `nonlocal` keywords are used to modify the scope of variables. They allow access to variables defined in outer scopes, such as global and enclosing (non-local) scopes, respectively. Here's how they work:

## Global Keyword

The `global` keyword is used inside a function to indicate that a variable being assigned to should have a global scope. It allows modifying a global variable from within a function. By default, if a variable is assigned a value within a function, Python considers it as a local variable. However, if you need to modify a global variable from within a function, you need to use the `global` keyword.

Usage example of `global` keyword:

```python
x = 10  # Global variable

def my_function():
    global x
    x = 20  # Modifying the global variable

my_function()
print(x)  # Output: 20
```

# Nonlocal Keyword

The nonlocal keyword is used inside a nested function to indicate that a variable being assigned to should have a scope in the nearest enclosing (non-local) scope, rather than creating a new local variable.

```python
def outer_function():
    x = 10  # Enclosing (non-local) variable

    def inner_function():
        nonlocal x
        x = 20  # Modifying the non-local variable

    inner_function()
    print(x)  # Output: 20

outer_function()
```

# Situations for Using global and nonlocal

The global keyword is useful when you want to modify a global variable from within a function. It allows you to access and update global variables directly.

The nonlocal keyword is useful when you have nested functions and need to modify variables from the nearest enclosing scope.

# Big O notation

Big O notation is an algorithm analysis to describe the performance and efficiency of an algorithm.
Enables developers to understand and compare the performance characteristics of algorithms.
# The Rolling Dice 
you can utilize the random module to generate a random number between 1 and 6, representing the faces of a standard six-sided die. 
1. We will just generate a random number from 1 to 6 with the package like this:
```python 
import random
print(random.randint(1,6)) 
```
