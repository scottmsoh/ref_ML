


## Regularization method (Avoiding overfitting)

Gap:
Lasso uses the absolute value of θi
Ridge uses the square value of θi

#### 1. L1 regularization (Lasso)

λ = is a regularization parameter (a hyperparameter)
θi = represents each coefficient in the model
equation: Cost function + λ * Sum of squares θi

-> Can set some coefficients to zero, effectively performing feature selection.
Useful when you have high-dimensional datasets (many features) and you suspect that only a few features are actually important

<span style="color:blue">only a few features to significantly influence the target variable</span>

<span style="color:blue">파란 글씨</span>

#### 2. L2 regularization (Ridge)

λ = is a regularization parameter (a hyperparameter)
θi = represents each coefficient in the model
equation: Cost function + λ * Sum of absolute value of θi

-> Tends to shrink coefficients but does not set them to zero.
Encourages the model to keep the coefficients as small as possible, which can help in handling multicollinearity and reducing model complexity.

<span style="color:blue"> many features are relevant or when you have multicollinearity in the data. </span>
