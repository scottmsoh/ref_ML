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

deicision_tree param (avoiding overfitting)
0(

랜덤서치
그리드서치는 범위 하나하나 다 적용 (속도 느림)
범위만 주면 여기서 랜덤으로 샘플을 뽑아서 진행 (다하면 느리므로 속도 빠름)
나머지 같으나 n-iter=100이 있음


## 3. Baysian Optimization

파라메터: (기계가) 역전파, 순전파 - 스캐일링, 쉬프트
하이퍼파라메타: (사람이) 뉴런의 개수, learning-rate 


