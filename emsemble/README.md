
### Ensemble model

1) Bagging (RandomForest) - 별도의 훈련세트 추출임? (훈련세트에서) - regression 모델에서도 쓸수있음
2) Boosting (XGBoost) - difference from Bagging. This will apply past prediction values
                        Previous prediction result affects to next predictions.
                        (샘플을 뽑을 때 잘못 분류된 data 50%를 재학습, 또는 가중치 이용)
4) Stacking (Combining two models)
5) Voting?
