

## PythonLGBM & S Scikit-learnLGBM 
(But mostly use Scikit-learnLGBM when we are friendly with Scikit-learn libarary)


## Most frequent-used Hyper Parameters
1. n_estimators(d=100) : the number of repeated execution (if it is bigger but it might be overfitting)
2. learning_rate(d=0.1)
3. Boosting_type
   1) GBDT(d)
   2) GOSS: Model will use the case when only Gradient value is big (Uncommon)
   3) DART: tree dropout (but longer execution time than others)

* Tree
4. max_depth(d=-1): depth, Leaf-wise method is much deeper than Level-wise
5. min_child_sample(min_data_in_leaf)(d=20): number of leaf-nodes (Uncommon)
6. num_leaves(d=31): number of max leafs per a tree

* Sampling
7. sub_sampling(bagging_fraction)(d=1.0) : row sampling
8. colsample_bytree(feature_fraction)(d=1.0) : column sampling

* Regularization
9. lambda_l2(reg_labda)
10. lambda_l1(reg_alpha)


------------------------------------------------------------------------------
## Search and optimization methods 
--> It is possible to tune manually parameters above, but there are useful methods
(method 1,2 are hard to apply previous tunned-results to next approaches but 3 is possible)

1. Grid Search
2. Random Search
3. Baysian Optimization (cross_validation)
- 
  
