# Linear Regression

## Model Representation
- Training set:
  - m = number of training examples
  - x = "input" variable / feature
  - y = "output" variable / "target" variable
  - (x, y) = one training example
  - (x<sup>(i)</sup>, y<sup>(i)</sup>) = ith training example
- Goal of a learning problem is to learn a function h(x) that is a good predictor for the corresponding value of y
- h = *hypothesis* function that takes input and returns an estimate
  - h<sub>theta</sub>(x) = theta<sub>0</sub> + theta<sub>1</sub>x
  - x, y have a linear relationship
  - Univariate linear regression

## Cost Function
- theta's are the parameters of the model
- Training set is used to fit h(x) closely to the data by choosing parameters theta<sub>0, 1</sub>
- Minimize cost function (sum squared error) over all training examples
- Cost function = J(theta<sub>0</sub>, theta<sub>1</sub>)
  - Squared error commonly used, good for most linear regression problems
  - Using the mean of the sum squared error, divided by 2 to simplify gradient descent calculation

## Parameter Learning
- Gradient descent
  - Chooses theta<sub>0</sub>, theta<sub>1</sub> to minimize cost function
  - Move parameters in the direction of deepest descent (partial derivative with respect to parameters)
- := assignment operator

![](https://www.codeproject.com/KB/recipes/879043/GradientDescent.jpg)
  
## Gradient Descent for Linear Regression
- [Deriving](http://mccormickml.com/2014/03/04/gradient-descent-derivation/) gradient descent
- Batch gradient descent
  - Each step of gradient descent uses all the training examples
  - i.e. the gradient is calculated by summing over all training data
