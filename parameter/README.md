
## Parameter Optimization
1. *Gradient Decent</br>
   - 전체 데이터 사용
2. *Stochastic Gradient Descent (SGD)</br>
   - Gradient Decent와 metrics는 동일하지만 한번 업데이트 시 일부데이터만 사용함 (시간,메모리 단축)
   - 일부데이터, 랜덤 미니배치 (stochastic이라는 단어 붙음)
   
4. Mini-Batch Gradient Descent</br>
5. Conjugate Gradient Descent</br>
6. Quasi-Newton Methods (like BFGS)</br>


Gradient Descent Methods
- STochastic gradient descent
![Image 2024-01-06 at 10 48 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/058b0ca0-9c8a-485e-959e-8c43b2ac6de7)

- Momentum
![Image 2024-01-06 at 10 47 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/fede7a48-ea1b-4631-bb04-a0dfbdd449cf)
  
- Nesterov accelerated gradient
![Image 2024-01-06 at 10 50 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/34feaefd-dbd3-4f78-8438-f8af52e230f6)

- Adagrad: Adapts the learning rate, performing larger updates for infrequent and smaller updates for frequent parameters.
![Image 2024-01-06 at 10 55 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/8b5ee20b-f85b-413a-81f9-f9f4b66a4a95)

- Adadelta: Learning rate 없어 잘 사용되지 않음
- ![Image 2024-01-06 at 11 05 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/fe760f70-b251-47f6-a198-28eba0e3cd7b)

![Image 2024-01-06 at 10 58 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/eaab6bfd-ae06-4e89-9ee4-8d9e482d6f7f)

- RMSprop: 많이 사용, is an unpublished, apaptive learning rate method proposed by Geoff Hinton in his lecture.
![Image 2024-01-06 at 11 02 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/5049f3f0-019f-4cb8-8240-8b93c7f85b87)

- Adam: 가장 많이 사용
![Uploading Image 2024-01-06 at 11.05 PM.jpeg…]()



W <- W - ng 
g: gradient (n = learning rate)

a <- Ba + g


