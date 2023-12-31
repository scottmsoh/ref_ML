## Performance evaluation metrics

#### Cross-validation technic</br>

accuracy_scores = cross_val_score(classifier, X, y, cv=5, scoring='accuracy')</br>
We can select methods such as accuracy or R square at the 'scoring' section.</br>


![Image 2023-12-25 at 4 17 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/4995674d-429f-4265-bed2-06f893f6cfa1)


### Classification Model

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
- MSE = 1/n * Sum of Squares (predicted value y - actual value y)</br>
- RMSE = Root 1/n * Sum of Squares (predicted value y - actual value y)</br>
- MAE = 1/n * Sum of absolute value (predicted value y - actual value y)</br>
- MARE (Mean Absolute Relative Error)</br>
   
   = 1/n * Sum of absolute value (predicted value y - actual value y) / actual value y

### Regression Model
   
5. R square
6. Adjusted R square
