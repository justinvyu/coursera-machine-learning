# Logistic Regression

- One of the most widely used classification algorithms
- Output *y* is mapped to discrete values
  - For example: {0, 1} where 0 is the "negative class" and 1 is the "positive class"
  - Works for binary and multiclass classification
- Logistic regression: 0 <= h<sub>theta</sub>(x) <= 1

## Model Representation

- Linear regression: h<sub>theta</sub>(x) = theta<sup>T</sup>x
- Logistic regression: using sigmoid function such that h<sub>theta</sub>(x) = 1 / (1 + e^-theta<sup>T</sup>x)
- Hypothesis output: h<sub>theta</sub>(x) = P(y = 1 | x; theta)
  - "probability that y = 1, given x, parameterized by theta"
- P(y = 1 | x; theta) + P(y = 0 | x; theta) = 1
  
## Decision Boundary

- Predict y = 1 whenever h<sub>theta</sub>(x) >= 0.5, or when theta<sup>T</sup>x >= 0
- Predict y = 0 whenever h<sub>theta</sub>(x) < 0.5, or when theta<sup>T</sup>x < 0
- Decision boundary is the line that separates the regions of y = 0 and y = 1
- Non-linear decision boundaries
  - Can add nonlinear features just like in linear regression

## Cost Function

- Least squares creates a non-convex cost function
- Thus, cost function is { -log(h<sub>theta</sub>(x)) if y = 1, -log(1 - h<sub>theta</sub>(x) if y = 0 }
  - Large (goes to infinity) penalty when h<sub>theta</sub>(x) = 0 when y = 1, as well as if h<sub>theta</sub>(x) = 1 when y = 0
  - Cost = 0 when h<sub>theta</sub>(x) and y match
- Cost(h<sub>theta</sub>(x), y) = -ylog(h<sub>theta</sub>(x)) - (1 - y)log(1 - h<sub>theta</sub>(x))

![](https://kousikk.files.wordpress.com/2014/11/screen-shot-2014-11-14-at-11-09-21-am.png)

## Gradient Descent

![](https://lotusthoughts.files.wordpress.com/2015/02/vlcsnap-2015-02-10-22h39m20s202.png)

## Advanced Optimization

- Conjugate descent, BFGS, L-BFGS
- Pick alpha for you, faster than gradient descent
- Create a function that calculates the cost given theta paremter and the gradient of the cost function (taking partial derivatives with respect to all parameter variables)
