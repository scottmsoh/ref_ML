<img src="https://capsule-render.vercel.app/api?type=모양&color=색상코드&height=높이&section=header&text=텍스트&fontSize=텍스트크기" />
* Methods

1. Grid Search
---------------------------------------------------------------
# Declaration
from sklearn.preprocessing import PolynomialFeatures
from sklearn.linear_model import LinearRegression
from sklearn.pipeline import make_pipeline
import matplotlib.pyplot as plt

* Start Grid search
from sklearn.model_selection import GridSearchCV
%matplotlib inline

param_grid = {'polynomialfeatures__degree': np.arange(21),
## range: 0~20 degree apply
              'linearregression__fit_intercept': [True, False],
              'linearregression__normalize': [True, False]}
## In this example: 20*2*2= 80ea number of cases  execution

grid = GridSearchCV(PolynomialRegression(), param_grid, cv=7)
## Cross-validation function: e.g. 7ea cross-validate

grid.fit(X,y)
grid.best_params_

## Optimized Model (plot visualization)
model = grid.best_estmiator_

plt.fiture(figsize=(8,7)
plt.scatter(X.ravel(), y)
lim = plt.axis()
y_test = model.fit(X,y).predict(X_test)
plt.plot(X_test.ravel(), y_test);
plt.axis(lim);

-----------------------------------------------------------------

2. Random Search
-----------------------------------------------------------------
dd





4. Baysian Optimization
