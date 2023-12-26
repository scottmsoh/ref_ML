
## How to overcome data imbalance

1. Augmentation
2. Specific sampling (under, over)
3. Weight loss function?(Pytorch) / Weighted randome sampling?
4. Ensemble model
5. Evaluation metrics (cross validation) - Accuracy, precision, recall, f1-score, ROC curve, AUROC


---- Imaga Processing Data Augmentation</br>
regularization,</br>
일반 classification과 달리</br>
pixel마다 sementic segmetation 의 경우 각각의 경우 정답이 필요함</br>
적용하기 어렵거나 안되는 경우도 있음</br>
Fistly normalization, 0~255 pxl 그대로 사용할 경우 큰 값에만 민감, 0~1로 normalize 해줌</br>
   --> 큰값 작은 값의 차이 존재, 평균값을 중간으로 혹인 0.5사용 (평균값을 빼고, 표준편차로 나눔=normalized)

1) Random flip and rotate
sementic, stereo matching pxl별로 정답이 있는 경우 X, 위치 정보 중요하므로
2) Cropping


-- Regression cases: Not really common
1) Noise Addition: Adding small amounts of noise to the input features can sometimes help prevent overfitting.
2) Feature Augmentation: Deriving new features based on existing ones (for example, creating polynomial features).
3) Bootstrapping

---- NLP Data Augmentation: NLTK
Altering the text data to create additional realistic training samples.

1) Synonym Replacement
2) Random Insertion
3) Random Swap
4) Random Deletion
5) Back Translation 
6) Text Surface Transformation

