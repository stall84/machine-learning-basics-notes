#### Cost (a.k.a. Loss) Function Basics

##### Things to consider in learning

- Algorithm performance is measured on 'unseen' test data (Standard method is to reserve about 20% of your training set/data to test on, leaving the larger 80% to train on)
- Performance measurement depends on the problem we are trying to solve: Meaning you can have your model underperform in some learning areas, as long as in the end it's solving the problem you originally sought to solve.
- There should be a strong connection between the training data and test data
- Formula: $l(\hat{y}, y)$ Where $\hat{y}$ is the predicted value, and $y$ is the truth, the function becomes a measurement of error.

#### Common Canonical Learning Problems

##### Regression

- Tries to predict a real value.
- Example: Predict the value of a stock tomorrow given it's past 3 month performance.
- Squared Loss Function: $l(\hat{y}, y) = (y - \hat{y})^2$
- Absolute Loss Function: $l(\hat{y}, y) = |y - \hat{y}|$

##### Binary Classification

- Tries to predict a simple yes/no response.
- Example: Predict whether a student will like a specific course or not.
- Zero/One Loss Function:
  $$
  f(x)=
  \begin{cases}
  1& \quad \text{if $y = \hat{y} $}\\
  0 & \quad \text{otherwise}
  \end{cases}
  $$

##### Multiclass Classification

- Predict which class (of many usually) an object (the thing being predicted) will belong to.
- Example: Predict whether a news story is about entertainment, sports, politics, religion, etc.
  $$
    f(x)=
    \begin{cases}
    1& \quad \text{if $y = \hat{y} $}\\
    0 & \quad \text{otherwise}
    \end{cases}
  $$
