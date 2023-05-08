# 1. Classes and objects in Python

##

- **Class**:

is a blueprint or template for creating objects.
It defines a set of attributes :<br>
`[variables,functions]
`

- **Object**:
 is an instance of a class. It represents a specific occurrence of the class.

## The differences between classes and objects in Python

 1. Definition:

- A class is defined using the class keyword, followed by the class name.
- An object is created by calling the class as if it were a function.

  2. Attributes:

- A class defines a set of attributes (variables) that describe the state of the objects created from it.
- An object created from the class has its own set of attribute values, which can be unique for each instance.

  3. Methods:

- A class also defines methods (functions) that define the behavior of the objects.
- An object created from the class can call the class's methods and execute the defined behavior.

  4. Inheritance:

- Classes in Python can inherit attributes and methods from other classes, forming a hierarchy of classes.
- Objects created from child classes have access to both the inherited methods and the specialized ones defined in the child class.

# 2. Recursion

It involves solving a problem by reducing it to one or more simpler instances of the same problem.

## Concept of a base case and a recursive case

- Base case : It defines the simplest form of the problem that can be solved directly without further recursion.
- Recursive case: It defines how the problem is reduced into a smaller subproblem or multiple subproblems.
Example:
```
def factorial(n):
if n == 0: `#Base case`
else:
return n * factorial(n - 1)`#Recursive case`
```
`Whice reduce the problem to a smaller subproblem`
### Best practices to follow when implementing a recursive function
- Define base case(s)
- Ensure progress towards the base case
- Manage function arguments.
- Avoid unnecessary computation
- Test with small inputs
- Consider performance
# Testing
Pytest fixtures and code coverage are two essential components in testing Python code that work together to enhance the quality and maintainab of a project.
 Pytest Fixtures:
 - provide a define and reusable set of test data or test resources for your test functions. 
 - Fixtures are defined as functions using the @pytest.fixture decorator. 
 They can be invoked in test functions by mentioning the fixture name as an argument.
- Code Coverage:is a metric that measures the extent to which your code is executed during testing,which helps in:
1. Identifying Uncovered Code
2. Guiding Test Development.
3. Quality Assurance.
code coverage analysis helps ensure that your tests are thorough and provides insights into areas of your code that need further testing.
