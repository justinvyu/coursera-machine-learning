# Multiclass Classification

- *y* can take on a set of discrete values
- One versus all classification
  - If there are 3 classes, turn classification into 3 different binary classification problems
  - Get decision boundaries for h<sub>theta</sub><sup>(i)</sup>(x) = P(y = i | x; theta) (i = 1, 2, 3, ...)
  - Train logistic regression classifier for each class
    - Pick the class that maximizes h<sub>theta</sub>(x), or the class that the value most likely falls under
