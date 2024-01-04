
```python


NLP Data Augmentation
NLTK Altering the text data to create additional realistic training samples.

ex) I love riding a bicyle.

Synonym Replacement: Replace words with synonyms. ex) I love taking motorcycle.
Random Insertion: Insert new words that are synonyms of words in the sentence. ex) I love riding a bicycle today.
Random Swap: Swap words in the sentence. ex) I ride love a bicycle.
Random Deletion: Randomly remove words. ex) Love riding a bicycle.
Back Translation: Translate the text to another language and then back to the original language. (High cost compared to performance, different results depending on each translator)
Text Surface Transformation: Apply surface-level changes, such as changing the tense or voice of sentences.

Data set (we can use sample)
SST-2 : stanford Sentiment Treebank
CR: customer reviews
SUBJ: subjectivity/objectivity dataset
TREC: question type dataset
PC: Pro-Con dataset

Models
LSTM - RNN
CNNs

EDA-data size별 overfitting
Data size 작으면 overfitting한다는 내용많음
실제 확인 히 EDA에 따른 영향도가 데이터 크기가 커질수록 커짐
EDA 진행한 문장이 레이블이 틀어지면 안되므로 잘 유지하는지에 대해 t-SNE 실험 (Dimension reduction)
EDA-original 그대로 유지되는지 검증
SR: a(원문 변화 비율)이 크면 오히려 성능 감소
RI: a 크더라도 성능 안정적으로 향상 (원래 단어와 그 관련된 순서들이 연산에서 유지)
RS, RD: a커지면 성능 변화가 커짐, 문장을 변형시키는 작업이라 성능 저하 피할수 없음
모든 작업에 대한 소규모 개선은 확실히 성능 향상에 기여 (a=0.1 sweet spot)

그렇다면 얼마나 augmentation하는게 좋을까?
적은 데이터셋의 경우 오버피팅이 발생 가능함, 문장을 많이 생성하면 큰 성능 향상 가능
ULMFit, ELMo, BERT 같은 모델에서는 무시할 수 있는 수준이라서 고민이 필요함


```
