
우리는 아이템을 bundle 추천이 목적</br>

## 평가함수 어떻게 선정?</br>

추천을 해준 영화를 봣는지 여부</br>
본 영화의 평점을 높이 줫는지 여부</br>

클릭 X. 유튜브는 체류시간을 본다고 함</br>

### 정확도: Accuracy (삿냐 안삿냐)</br>
   추천한것, 추천하지 않은 것 맞았는지 둘다 확인 필요하나 추천하지않은 것은 너무 많음</br>
   20개 이상 추천, 먼저 추천해준게 좋고,</br>
   Map(먼저 뒤 추천 좋은 여부가 있음)</br>

1) Map(precision의 AVG를 구한값)</br>

   ![Image 2024-01-02 at 4 18 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/d2fb988a-3c5b-4557-bfe7-d38731965da6)

2) NDCG (Cumulative Gain)
   


Cross-validation: K fold and average of performance data
validation 5개의 평균 = 나머지 셋트끼리의 평균?
X_poly, Y = shuffle(X_poly, Y) // Shuffle 필요 (Randomly choosing)

Comparison with Training Performance: If a model has much higher performance on its training set compared to its cross-validation score, this is a sign of overfitting. The model is learning the training data too closely but not generalizing well to new data.

비지도 방식 NN than KNN


