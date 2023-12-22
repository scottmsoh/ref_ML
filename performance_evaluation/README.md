## Performance evaluation metrics

#### Classification Model

Confusion matrix

![KakaoTalk_Photo_2023-12-22-10-39-20](https://github.com/scottmsoh/ref_ML/assets/112598791/250bd658-168f-4dae-adba-e6912a916a90)

1) Precision: TP/TP+FP 
2) Recall(=Sensitivity): TP/TP+FN
3) Specificity: TN/FP+TN
4) F1-score: 2 * (Recall*Precision / Recall+Precision) 
5) ROC curve: 
6) AUROC: the area under the ROC curve.
An AUROC of 1 indicates a perfect classifier, while an AUROC of 0.5 indicates a worthless classifier. A higher AUROC value indicates a better overall performance of the classifier.

7) Accuracy
1. MSE = 1/n * Sum of Squares (predicted value y - actual value y)
2. RMSE = Root 1/n * Sum of Squares (predicted value y - actual value y)
3. MAE = 1/n * Sum of absolute value (predicted value y - actual value y)
4. MARE (Mean Absolute Relative Error) 
   
   = 1/n * Sum of absolute value (predicted value y - actual value y) / actual value y


#### Regression Model
   
5. R square
6. Adjusted R square


