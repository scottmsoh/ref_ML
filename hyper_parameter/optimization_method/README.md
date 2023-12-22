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
실험데이터에 노이즈 (outlier or missing values) 껴있는 경우 사용한다
목적 함수에 대한 아무런 정보가 없을 떄 사용

1) 주어진 데이터에서 랜덤하게 샘플링을 한다.
2) 샘플들로부터 surrogate function을 계산한다.
3) surrogate function으로부터 획득함수(Aquisition function)을 최대화 하는 새로운 샘플값을 추가한다.
4) surrogate function을 다시 계산한다.
5) surrogate function의 최대값이 안바뀌거나 분산이 역치 이하이면 반복계산하는것 중지한다.


## 4. AutoML



