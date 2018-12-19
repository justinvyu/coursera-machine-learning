# Multivariate Linear Regression

## Multiple Features

- n = number of features
- x<sup>(i)</sup> = input (features) of ith training example
  - x<sup>(i)</sup> becomes a vector
- x<sub>j</sub><sup>(i)</sup> = value of feature j in ith training example
- Hypothesis: h<sub>theta</sub>(x) = theta<sub>0</sub> + theta<sub>1</sub>x<sub>1</sub> + theta<sub>2</sub>x<sub>2</sub> + ...
- theta = (n+1)-dimensional vector for parameters
  - Hypothesis becomes h<sub>theta</sub>(x) = theta<sup>T</sup>x
  
## Gradient Descent

![](http://www.holehouse.org/mlclass/04_Linear_Regression_with_multiple_variables_files/Image%20[3].png)

## Feature Scaling

- Gradient descent can converge more quickly if features are on a similar scale
- Often want to get every feature into approximately a -1 <= x<sub>i</sub> <= 1
  - Not exact requirements, just meant to speed things up
- Mean normalization (sort of like calculating a z-score) where you make features have approximately zero mean by subtracting the average value and dividing by the range

## Learning Rate

- "Debugging" or making sure gradient descent is working correctly
  - Plot cost function vs # of iterations as gradient descent runs
  - J(theta) should **decrease** after every iteration
  - Example convergence test: declare convergence if J(theta) decreases by less than 10<sup>-3</sup> in one iteration (error)
- Choosing the right alpha (learning rate)
  - If J(theta) vs # of iterations plot shows that the cost function is increasing / sporadic, use a smaller alpha
  - If alpha is too small, gradient descent can be too slow to converge
  - Try powers of 10 (0.001, 0.01, 0.1, 1, ...)
  
## Features and Polynomial Regression

- Can create new features using operations on given features
- Set higher degree terms to new features
  - Allows you to fit to quadratic/cubic/higher power models
