
## Feature_selection methods


![Image 2023-12-22 at 10 35 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/a5b89218-80fc-413c-afc2-f527b55d2353)


1. Filter method</br>
   1) Correlation-Coefficient (Create heatmap corr matrix to select relevant features)</br>
   2) Chi-square test: 변수가 많을때</br>
   3) ANOVA</br>
   4) Information Gain</br>

2. Wrapper method (ML model-tree model) : 단점 시간 오래걸림, 비용 소요</br>
   AIC? 낮을 수록 좋음, R square 1에 가까울수록, F-statistics 클수록</br>
   subset을 만들어 돌리고 점차 1,2,3개 늘려가면서 모델 성능 측정</br>
   
   1) Forward Selection: Add larger correlation coeff first (lower p-value)</br>
   2) Backward Elimination: Add every feature and deduct one by one (bigger p-value)</br>
   3) Stepwise Selection: Mixed Forward and Backward</br>

3. Embedded methods</br>
   1) Lasso regression</br>
   2) Elastic Net</br>
   3) Ridge regression</br>
      
---------------------------------------------------------------
1. Demension Reduction = Feature extraction</br>
  1) PCA (Principle Component Analysis)</br>
  2) LDA (Linear Discriminant Analysis)</br>
  3) t-SNE (t-Distributed Stochastic Neighbor Embedding)</br>
  4) </br>

2. 
