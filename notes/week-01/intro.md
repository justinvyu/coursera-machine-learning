# Introduction

## Supervised Learning
- Supervised learning problems will provide the "right answers" to given inputs.
- **Regression problem** = predict results of a continuous output
- **Classification problem** = predict results of a discrete output
  - Returns a discrete output (i.e. 0 or 1)
  - Mapping input variable to discrete categories
  - Can also have more than 2 values for output (i.e. return 0, 1, 2, 3...)
- **Features** (attributes) are used to classify between datasets
  - Example: Age and Tumor Size are both features used to determine whether a tumor is malignant or benign
  - Sometimes you want to use an infinite number of features -> SVM

## Unsupervised Learning
- Given **unlabeled** data
- Determining clusters in data without given any prior knowlege of the data
- Allow the algorithm to discover patterns & relationships
- No feedback on prediction results
- Example: Cocktail party algorithm
  - Separating a sum of data (singling out one voice from a recording)
