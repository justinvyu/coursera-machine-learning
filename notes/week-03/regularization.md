# Regularization

## Overfitting

- Underfitting = "high bias"
- Overfitting = "high variance"
  - Overfitting comes when there are too many features that fits the training set very well but fails to generalize new examples
  - Hypothesis is unlikely to predict for new examples
- Addressing overfitting
  - Reducing number of features
    - Manually select which to keep
    - Model selection algorithms
  - Regularization
    - Keep all features, but reduce magnitudes/values of parameters theta<sub>j</sub>
    - Works well with lots of features

## Regularized Linear Regression

- Small values for parameters
  - Simpler hypothesis, less prone to overfitting
  - ![](http://www.holehouse.org/mlclass/07_Regularization_files/Image%20[5].png)
  - Add term at the end of cost function
    - Lambda = regularization parameter, controls between training well and keeping values small
    - Large lambda values means that the model will be underfit
- Multiplying parameters by a scalar that is a usually a little bit less than 1 (shrinking) then subtracting the cost gradient just like in linear regression

## Regularized Logistic Regression

- Same cosmetically as linear regression
- Skips penalizing theta<sub>0</sub> by only adding a regularization term for j = 1 - n
