
### Ensemble model

1) Bagging (RandomForest) - 별도의 훈련세트 추출임? (훈련세트에서) - regression 모델에서도 쓸수있음
2) Boosting (XGBoost) - difference from Bagging. This will apply past prediction values
                        Previous prediction result affects to next predictions.
                        (샘플을 뽑을 때 잘못 분류된 data 50%를 재학습, 또는 가중치 이용)
4) Stacking (Combining two models)
5) Voting - soft voing 구분 / hard voting (투표용지)
   soft voting - confidence value

![Image 2023-12-25 at 10 27 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/8fb3c1d9-21b6-4844-b248-a88b1142677f)

   
