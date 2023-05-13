# `random` Generate pseudo-random numbers

The random module in Python is a built-in module that provides functions for  <br><br>

|1. Generating random numbers | 3. Making random selections |
|2. Shuffling sequences       | 4. random related operations|

How you can use the random module:

1. Importing the module:
To use the random module, you need to import it at the beginning of your Python script or interactive session:<br>
`import random
`
2. Generating random numbers:
The random module provides several functions to generate random numbers. <br>
Some commonly used functions are:

- `random()`: Returns a random float number between ( 0-1 )(inclusive of 0, exclusive of 1).
- `randint(a, b)`: Returns a random integer between a and b (inclusive of both a and b).
- `uniform(a, b)`: Returns a random float number between a and b (inclusive of both a and b).
- `randrange(start, stop, step)`: Returns a randomly selected element from the range created by the arguments. Similar to range(), but the values are randomly chosen.

3. Making random selections:
The random module allows you to make random selections from a list, sequence, or any iterable. Here are a few functions for making selections:

- choice(sequence): Returns a randomly selected element from the given sequence.
- sample(population, k): Returns a randomly selected sample of k elements from the given population (which can be a list, set, or any iterable).
- shuffle(sequence): Randomly shuffles the elements in the given sequence in place (modifies the original sequence).

4. Setting the random seed:
If you want to generate the same sequence of random numbers each time you run your program, you can set a random seed using random.seed().

# Risk Analysis in Software Testing

Risk analysis refers to the process of identifying, assessing, and prioritizing potential risks that may affect the success of a software project.
The goal of risk analysis is to proactively address potential issues to increase the chances of project success.
The key steps involved in conducting a risk analysis for a software project:

1. Risk Identification
2. Risk Assessment
3. Risk Analysis
4. Risk Response Planning
5. Risk Monitoring and Control
6. Documentation and Communication

### Test coverage is a metric used in software testing to measure the extent to which the source code of a software system is tested by a set of test cases

Test coverage is often expressed in terms of statements, branches, conditions, or paths covered by the tests.
Test coverage is an important metric in software testing for several reasons:

1. Quality Assessment, test coverage helps assess the thoroughness of testing efforts.

2. Risk Identification, By identifying areas of the code that lack coverage, test coverage can help pinpoint potential vulnerabilities or untested scenarios.
3. Requirement Fulfillment: Test coverage can be linked to software requirements, enabling the evaluation of how well the tests address the specified functional and non-functional requirements.
4. Code Maintenance: Test coverage provides insights into the maintainability of the codebase.

# Big O notation

Big O notation is a mathematical notation used to describe the performance or efficiency of an algorithm. It represents the upper bound or worst-case scenario of how the algorithm's runtime or space requirements grow as the input size increases.

In Big O notation, "O" stands for order, and it is followed by a function that represents the growth rate of the algorithm. The function typically describes the relationship between the input size (n) and the algorithm's time complexity or space complexity.
