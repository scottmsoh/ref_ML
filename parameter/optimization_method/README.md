# Methods

## 1. Grid Search

## 2. Random Search

훈련세트: 훈련에 사용
검증세트: 각 메소드의 하이퍼파라메터 검증할때 사용
테스트: 예측 시 한번만 사용

단순하게 하는 방법은 : 훈련세트 60%, 검증 20%, 테스트 20%
But sklearn의 5fold cross-validation (d=5) 주로 사용
훈련/훈련/검증
훈련/검증/훈련 --> 검증 점수 평균
검증/훈련/훈련 

cv=옵션객체,
stratifiedKfold(n_splits=5, shuffle(d=False)=True, random_state=42)
scores = cross_validate(dt, train_input, train_target, return_train_score=True, cv=splitter)


## 3. Baysian Optimization
