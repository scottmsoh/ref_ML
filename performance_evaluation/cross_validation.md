
Cross-validation: K fold and average of performance data</br>
validation 5개의 평균 = 나머지 셋트끼리의 평균?</br>
X_poly, Y = shuffle(X_poly, Y) // Shuffle 필요 (Randomly choosing)</br>

Comparison with Training Performance: If a model has much higher performance on</br>
its training set compared to its cross-validation score, this is a sign of overfitting.</br>
The model is learning the training data too closely but not generalizing well to new data.</br>

