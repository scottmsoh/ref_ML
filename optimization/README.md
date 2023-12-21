# Methods

## 1. Grid Search
---------------------------------------------------------------
- Declaration
from sklearn.preprocessing import PolynomialFeatures
from sklearn.linear_model import LinearRegression
from sklearn.pipeline import make_pipeline
import matplotlib.pyplot as plt

* Start Grid search
from sklearn.model_selection import GridSearchCV
%matplotlib inline

param_grid = {'polynomialfeatures__degree': np.arange(21),
<h1> annotation range: 0~20 degree apply </h1>
              'linearregression__fit_intercept': [True, False],
              'linearregression__normalize': [True, False]}
<h1> annotation In this example: 20*2*2= 80ea number of cases  execution </h1>

grid = GridSearchCV(PolynomialRegression(), param_grid, cv=7)
<h1> annotaion Cross-validation function: e.g. 7ea cross-validate </h1>

grid.fit(X,y)
grid.best_params_

* Optimized Model (plot visualization)
model = grid.best_estmiator_

plt.fiture(figsize=(8,7)
plt.scatter(X.ravel(), y)
lim = plt.axis()
y_test = model.fit(X,y).predict(X_test)
plt.plot(X_test.ravel(), y_test);
plt.axis(lim);

-----------------------------------------------------------------

## 2. Random Search
-----------------------------------------------------------------
dd





## 3. Baysian Optimization
