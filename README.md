# ECE2112-2ECEC-PA2

Made by Shaun Michael R. Remular

This Repository contains the Programming Assignment 2 for the course "Advanced Computer Programming" S.Y. 2026-2027. This project covers Module 2- Numerical Python, including three Python problems.

## Objectives
1. Use Numerical Python (Numpy) and ndarrays in problem solving
2. Apply Numpy to solve problems relating to matrices

The code imports Numerical Python (Numpy) as np

## A. Reproducible Normalization Problem
The Reproducible Normalization problem involves a 5x5 integer ndarray that was then normalized. Wherein the mean of the normalized array is 0, while the Standard deviation is 1.

- ````____.mean()```` was used to generate the mean of the array.
- ````____.std()```` was used to generate the standard deviation of the array.

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

The resulting answer was then saved as a .npy file
using ````np.save(____,____)````

## B. Cubes Divisible by 4 Problem
The Cubes Divisible by 4 Problem involves creating a 10 x 10 array containing the first one hundred perfect cubes. Using a Boolean condition, the array was filtered to obtain only the perfect cubes divisible by 4.

- ````np.arange```` was used to generate the array containing the perfect cubes.
- ````__.reshape```` was used to reshape the array into a 10 x 10 array.

The following codes were then used in order to generate the array.
````
C = (np.arange(1,101,1)**3).reshape(10,10)
C
````

Following the generation of the array, the modulus of the array was taken, keeping only true values or values that are divisible by 4.
````
div_by_4 = C[C%4==0]
````
The resulting answer was then saved as a .npy file
using ````np.save(____,____)````

## C. Above-Mean Squares
The Above-Mean Squares problem involves taking the mean of a 6 x 6 array containing the first thirty-six perfect squares. The array's mean was then used to filter out numbers less than the mean, leaving only those greater than it.

The following code was then used to generate the array.
````
S = (np.arange(1,37,1)**2)
S
````

Afterward, similar to the first problem, the mean was taken.
````
S_mean = S.mean()
S_mean
````

And lastly, similar to the second problem, the array was filtered out, keeping only the true values or the values that were greater than the mean.
````
above_mean = S[S>S_mean]
above_mean
````

The resulting answer was then saved as a .npy file
using ````np.save(____,____)````



README File Version History

September 3, 2026 - Preliminary

September 3, 2026 - Additional Info
