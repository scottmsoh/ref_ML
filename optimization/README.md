# Methods

## 1. Grid Search
---------------------------------------------------------------
- Declaration <br/>
from sklearn.preprocessing import PolynomialFeatures <br/>
from sklearn.linear_model import LinearRegression <br/>
from sklearn.pipeline import make_pipeline <br/>
import matplotlib.pyplot as plt <br/><br/>

* Start Grid search <br/>
from sklearn.model_selection import GridSearchCV <br/>
%matplotlib inline <br/>

param_grid = {'polynomialfeatures__degree': np.arange(21),
<h3> annotation range: 0~20 degree apply </h3>
              'linearregression__fit_intercept': [True, False],
              'linearregression__normalize': [True, False]}
<h3> annotation In this example: 20*2*2= 80ea number of cases  execution </h3>

grid = GridSearchCV(PolynomialRegression(), param_grid, cv=7)
<h3> annotaion Cross-validation function: e.g. 7ea cross-validate </h3>

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
