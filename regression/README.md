


## Regularization method (Avoiding overfitting)

Gap:</br>
Lasso uses the absolute value of θi</br>
Ridge uses the square value of θi</br>

#### 1. L1 regularization (Lasso)
---------------------------------------------------------------------------
λ = is a regularization parameter (a hyperparameter)</br>
θi = represents each coefficient in the model</br>
equation: Cost function + λ * Sum of absolute value of θi</br>

-> Can set some coefficients to zero, effectively performing feature selection.
Useful when you have high-dimensional datasets (many features) and you suspect that only a few features are actually important</br>

### only a few features to significantly influence the target variable
---------------------------------------------------------------------------


#### 2. L2 regularization (Ridge)
---------------------------------------------------------------------------
λ = is a regularization parameter (a hyperparameter)</br>
θi = represents each coefficient in the model</br>
equation: Cost function + λ * Sum of squares θi</br>

-> Tends to shrink coefficients but does not set them to zero.</br>
Encourages the model to keep the coefficients as small as possible, which can help in handling multicollinearity and reducing model complexity.</br>

### many features are relevant or when you have multicollinearity in the data
---------------------------------------------------------------------------
