# Mathematical Statistics Functions

This module provides functions for calculating mathematical statistics of numeric (Real-valued) data. It includes functions for calculating averages, measures of central location, measures of spread, and statistics for relations between two inputs. The module supports int, float, Decimal, and Fraction data types.

## Averages and Measures of Central Location

- `mean()`: Calculates the arithmetic mean (average) of the data.
- `fmean()`: Calculates the arithmetic mean of the data, with optional weighting.
- `geometric_mean()`: Calculates the geometric mean of the data.
- `harmonic_mean()`: Calculates the harmonic mean of the data.
- `median()`: Calculates the median (middle value) of the data.
- `median_low()`: Calculates the low median of the data.
- `median_high()`: Calculates the high median of the data.
- `median_grouped()`: Calculates the median of grouped data.
- `mode()`: Calculates the single mode (most common value) of discrete or nominal data.
- `multimode()`: Calculates the list of modes (most common values) of discrete or nominal data.
- `quantiles()`: Divides the data into intervals with equal probability.

### Measures of Spread

- `pstdev()`: Calculates the population standard deviation of the data.
- `pvariance()`: Calculates the population variance of the data.
- `stdev()`: Calculates the sample standard deviation of the data.
- `variance()`: Calculates the sample variance of the data.

### Statistics for Relations Between Two Inputs

- `covariance()`: Calculates the sample covariance for two variables.
- `correlation()`: Calculates Pearson's correlation coefficient for two variables.
- `linear_regression()`: Calculates the slope and intercept for simple linear regression.

The functions in this module do not require the data to be sorted. The module also provides examples and usage details for each function.

# Basic Statistics in Python — Probability

This repository provides examples and code snippets for performing basic statistics and probability calculations in Python.

## Contents

1. [Generating Random Numbers](#generating-random-numbers)
2. [Calculating Factorial](#calculating-factorial)
3. [Calculating Permutations and Combinations](#calculating-permutations-and-combinations)
4. [Calculating Probability Distributions](#calculating-probability-distributions)
5. [Simulating Random Variables](#simulating-random-variables)

---

## Generating Random Numbers

To generate random numbers, you can use the `random` module in Python. Here's an example of generating a random number between 0 and 1:

```python
import random

random_number = random.random()
print(random_number)

```

## Calculating Factorial

The factorial of a number can be calculated using the math module in Python. Here's an example:

```python
import math

factorial_result = math.factorial(5)
print(factorial_result)
```

## Calculating Permutations and Combinations

The math module provides functions for calculating permutations and combinations. Here are a couple of examples:

```python
import math

# Permutations
n = 5
r = 3
permutations = math.perm(n, r)
print(permutations)

# Combinations
n = 5
r = 3
combinations = math.comb(n, r)
print(combinations)
```

## Calculating Probability Distributions

You can use various libraries like scipy or numpy to work with probability distributions. Here's an example of calculating the probability density function (PDF) of a normal distribution using scipy:

```python
from scipy.stats import norm

mean = 0
std_dev = 1

x = 1
pdf = norm.pdf(x, mean, std_dev)
print(pdf)
```

## Simulating Random Variables

You can simulate random variables from probability distributions using libraries like numpy or scipy. Here's an example of generating random samples from a normal distribution:

```python
import numpy as np

mean = 0
std_dev = 1

samples = np.random.normal(mean, std_dev, 1000)
print(samples)
```
