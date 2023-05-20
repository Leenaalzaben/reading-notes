# Python – List Comprehension

A Python list comprehension consists of brackets containing the expression, which is executed for each element along with the for loop to iterate over each element in the Python list.

## Python List Comprehension Syntax

`newList = [expression (element) for element in oldList if condition]`<br>
Python List comprehension provides a much more short syntax for creating a new list based on the values of an existing list.

## Advantages of List Comprehension

- More time-efficient and space-efficient than loops.
- Require fewer lines of code.
- Transforms iterative statement into a formula.

### Iteration with List comprehension example

```python
# Using list comprehension to iterate through loop
List = [character for character in [1, 2, 3]]

# Displaying list
print(List)
 
```

The Output will be
 > [1, 2, 3]

# Decorators in Python

 Decorators are a very powerful and useful tool in Python since it allows programmers to modify the behaviour of a function or class.
 Decorators allow us to wrap another function in order to extend the behaviour of the wrapped function, without permanently modifying it.

 Decorators are denoted by the ` @ ` symbol followed by the decorator function name placed above the definition of the function or class being decorated. When the decorated function or class is invoked, it is actually the decorator function that gets executed first, and it can decide whether to modify, replace, or wrap the original function or class.

# The concept of decorators in Python

Decorators in Python are a way to modify or enhance the behavior of functions or classes without directly changing their source code. <br>
They allow you to wrap a function or class with another function, commonly known as a decorator function, which can add extra functionality, modify inputs or outputs, or perform other actions before or after the decorated function or class is executed.<br>
The basic idea behind decorators is that they take a function (or class) as input, create a new function that usually extends or modifies the behavior of the original one, and returns this new function.

### Common use cases for decorators include

- Adding logging statements before and after the execution of a function to track its behavior.
- Measuring the time taken by a function to execute.
- Checking the inputs or outputs of a function to ensure they meet certain criteria.
- Storing the results of expensive function calls and returning them directly for subsequent identical calls.
- Implementing access control mechanisms for functions or classes.
- Adding additional debugging information or error handling to functions.

## Examples

1.`log_decorator`

```python
def log_decorator(func):
    def wrapper(*args, **kwargs):
        print(f"Calling function {func.__name__} with args {args} and kwargs {kwargs}")
        return func(*args, **kwargs)
    return wrapper

@log_decorator
def add(x, y):
    return x + y

add(2, 3) 
# Output: Calling function add with args (2, 3) and kwargs {}
         #         5

```

2. `time_decorator`

```python
import time

def time_decorator(func):
    def wrapper(*args, **kwargs):
        start_time = time.time()
        result = func(*args, **kwargs)
        end_time = time.time()
        print(f"Function {func.__name__} took {end_time - start_time:.2f} seconds to execute")
        return result
    return wrapper

@time_decorator
def slow_function():
    time.sleep(2)

slow_function() 
# Output: Function slow_function took 2.00 seconds to execute

```

3. `cache_decorator`

```python
def cache_decorator(func):
    cache = {}
    def wrapper(*args):
        if args in cache:
            print(f"Returning cached result for args {args}")
            return cache[args]
        else:
            result = func(*args)
            cache[args] = result
            print(f"Caching result for args {args}")
            return result
    return wrapper

@cache_decorator
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

fibonacci(10) # Output: Caching result for args (0,)
              #         Caching result for args (1,)
              #         Caching result for args (2,)
              #         Caching result for args (3,)
              #         Caching result for args (4,)
              #         Caching result for args (5,)
              #         Caching result for args (6,)
              #         Caching result for args (7,)
              #         Caching result for args (8,)
              #         Caching result for args (9,)
              #         Caching result for args (10,)
              #         55

```
