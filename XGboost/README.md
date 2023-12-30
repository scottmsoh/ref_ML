# XGBoost
XGBoost

* Do not have to fill the Null, missing values

![Image 2023-12-30 at 1 19 AM](https://github.com/scottmsoh/ref_ML/assets/112598791/bab31583-b099-42d2-9fbb-eaf9be8aae2a)


* Parameters tunning:
1) max_depth(d=6):
2) n_estimator(d=100): 500, 1000
3) early_stopping_round(d= x): 5
1) subsample = 0.75 e.g. row sampling
2) gamma(d=0): 0.25 e.g. increase gamma -> less splits / less complex (reduce overfitting)
3) learning rate(d=0.3): 0.05 (it should be runned together with the number of trees)
   --> Gradient decent (Find slope=0)

![gradient_decent](https://github.com/scottmsoh/ref_ML/assets/112598791/41a14340-462d-480a-a52a-70385edea3ae)

   
5) n_jobs(d=?): 4
6) reg_alph(d=0) = l1 regularization
7) reg_lambda(d=1) = l2 regularization


* Hyper parameters
Methods
1) Grid search
2) Random search

![Image 2023-11-05 at 9 45 PM](https://github.com/scottmsoh/XGBoost/assets/112598791/04ea074f-1ba3-4b63-a15e-f25608579681)

![Image 2023-11-05 at 9 59 PM](https://github.com/scottmsoh/XGBoost/assets/112598791/7edede6f-6b2c-41cb-977f-14191cfd6ff3)

