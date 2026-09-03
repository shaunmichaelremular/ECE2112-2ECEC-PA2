# ECE2112-2ECEC-PA2

Made by Shaun Michael R. Remular

This Repository contains the Programming Assignment 2 for the course "Advanced Computer Programming" S.Y. 2026-2027. This project covers Module 2- Numerical Python, including three Python problems.

## Objectives
1. Use Numerical Python (Numpy) and ndarrays in problem solving
2. Apply Numpy to solve problems relating to matrices

## A. Reproducible Normalization Problem
The Reproducible Normalization problem involves a 5x5 integer ndarray that was then normalized. Wherein the mean of the normalized array is 0, while the Standard deviation is 1.

The code below was used to generate the 5x5 integer ndarray
````
np.random.seed(2112)
X = np.random.randint(10, 101, size=(5, 5))
X
````

The code used in order to normalize the whole array uses the formula Z = (X-x)/σ. 
````
X_normalized = (X-X.mean())/X.std()
X_normalized
````

The mean and the standard deviation of the normalized array 'X_normalized' were then taken.
````
X_normalized.mean()
round(X_normalized.std())
````

## B. Cubes Divisible by 4 Problem





## C. Above-Mean Squares


README File Version History

September 3, 2026 - Preliminary
