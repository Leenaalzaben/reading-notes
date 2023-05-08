# Reading and Writing Files in Python

## 1. Opening and Closing a File in Python

When you want to work with a file, the first thing to do is to **open it**.
This is done by invoking the `open() built-in function`.<br>
 open() has a single required argument that is the path to the file.
 open() has a single return, the file object:<br>
 `file = open('dog_breeds.txt')`.<br>
 The next thing is how to **close it**.
There are two ways that you can use to ensure that a file is closed properly, even when encountering an error. The first way to close a file is to use the try-finally block:

`reader.close()
`

## The `with` statement: The second way to close a file

**with open(.txt) as reader** <br>
The `with` statement automatically takes care of closing the file once it leaves the with block, even in cases of error.

In Python, the with statement is used in conjunction with file operations to ensure that resources are managed properly. It provides a convenient way to handle file objects and guarantees that they are properly closed after use, even if an exception occurs.

 `with open(filename, mode) as file:`

`with` can avoid common pitfalls such as forgetting to close a file or handling exceptions related to file operations. It promotes cleaner and safer file handling practices in Python.

## 2. The difference between the '`read()`' and '`readline()`' methods

- Two methods for reading data:

- read() method:
 Used to read a specified number of bytes from a file, or if no size is specified, it reads the entire contents of the file. It returns the data as a string.
 Example ==>

 ```
with open('file.txt', 'r') as file:
    data = file.read()
    print(data)



 ```

Use read() when:

1. You want to read the entire contents of a file as a single string.
2. The size of the file is small enough to fit comfortably in memory.
3. You need to manipulate or process the entire contents of the file at once.

- readline() method:
 Used to read a single line from a file at a time. It returns the line as a string, including the trailing newline character.

Example ==>

```
with open('file.txt', 'r') as file:
    line = file.readline()
    while line:
        print(line)
        line = file.readline()


```

Use readline() when:

1. You want to process a file line by line, rather than reading the entire file at once.
2. The file is large and reading it all at once may exceed available memory.
3. You need to perform specific operations on each line individually.

## 3.  Use `try`, `except`, and optionally `finally`

- The `try` block is used to enclose the code that might raise an exception.
- The `except` block specifies the code that should be executed if a specific exception occurs within the try block.
- The `finally` block, if present, is executed regardless of whether an exception occurred or not. It is often used to perform cleanup operations or release resources.<br>
Example ==>

```
try:
  print(x)
except:
  print("Something went wrong")
finally:
  print("The 'try except' is finished")
```
