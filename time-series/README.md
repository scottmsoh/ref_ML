

![Image 2024-01-13 at 10 51 AM](https://github.com/scottmsoh/ref_ML/assets/112598791/88e7e534-ddab-419f-b0a5-7e23c0ff0c90)



ARIMA - seasonal, univariate case</br>
1. AR: Auto regression (과거를 정보로 활용)</br>
2. I: 차분 (불규칙성을 보완, 경향성)</br>
3. MA: moving average (이동 평균: 이전 항에서의 오차를 참고)</br>
model = ARIMA(name_of_df.values, order = (2,1,2)) or (0,1,2) = AR=2, I=1. MA=2</br>

규칙적, 불규칙적 방법</br>
supervised learning</br>
시계열은 특정시점으로 -5일 : train, +5일 : test</br>


Facebook Prophet</br> 
conda install -c conda-forge fbprophet (별도 설치필요)</br>
강점: seasonality_mode='multiplicative'</br>
yearly_seasonality=True</br>
weekly_seasonality=True</br>
daily_seasonality=True</br>
changepoint_prior_scale=0.5</br>


모델 더 디벨롭하는 과정</br>

1. 상한가, 하한가 설정 (cap=?)</br>
2. 이상치 제거</br>



