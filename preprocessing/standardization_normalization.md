

#### Nomalization / Standardization

- Regression models
  1) Linear-regression: Required but Standardization is recommended </br>
  2) Lasso, Ridge: Do not need nomalization (Regularize themselves)</br>
  3) Decision Tree, RandomForest: Do not need nomalization (Random sampling)</br>
  4) XGBoost, LGBM: Do not need</br>


- Classification models
  1) Logistic-regression: Required, sensitive to scale
  2) SVM: Highly recommended, sensitive to scale
  3) kNN: Essential, because features on larger scales can dominate the distance calculation
  4) Neural Networks: Highly recommended, speeding up the training process and avoiding issues with activation functions.
  5) Tree-based: Not necessary.
  6) Naive Bayes: Depends on the variant

