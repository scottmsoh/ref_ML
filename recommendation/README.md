

추천시스템
1. 브런치 - 관련글 추천
2. 당근 - 본 제품을 같이 봤던 고객이 어떤 상품을 같이 봤는지

3. 

![Image 2023-12-28 at 12 21 AM](https://github.com/scottmsoh/ref_ML/assets/112598791/a3fc588d-9508-4c28-b5f3-40af695e3662)

## Memory-Based Methods = neighborhood-based: KNN

### User-based Collaborative filltering : 
- 좋아요 (1,0)
- 영화별, 제품 별 0,1 marking
- Cosine similarity : 두 user의 좋아요 True/False value를 곱해서 나온값을 더함
- rows: 유저별, columns: 영화별

### Item-based Collaborating filtering
- 스파이더맨과 비슷한 영화가 어떤건지 알면 추천 가능 ex) 게츠비
- rows: 영화별, columns: 유저별 (반대)
- Cosine similarity : 두 user의 좋아요 True/False value를 곱해서 나온값을 더함

### Content-based filtering
- 하지만 새로운 영화 출시? (위 두가지로는 불가)
- 새로운 영화 좋아요 없음 (cold-start)
- Content-based로 가능
- 새로운 features 생성해야함 (아이언맨 영화, 디카프리오 출연, 실제스토리...)


![Image 2023-12-28 at 5 43 PM](https://github.com/scottmsoh/ref_ML/assets/112598791/b3973774-74ca-4fc6-a7ff-13d2cdf300c9)

-

## Model-based Methods

ALS (Alternating Least Squares):
Category: Model-Based Method
Details: ALS is used in matrix factorization, which is a model-based approach. It works by decomposing the user-item interaction matrix into lower-dimensional matrices representing latent factors for users and items. ALS alternates between fixing the user factors and solving for item factors, and vice versa, which makes it suitable for handling implicit feedback datasets and scalable for large datasets.

SGD (Stochastic Gradient Descent):
Category: Model-Based Method
Details: SGD is an optimization technique that can be used in various model-based collaborative filtering algorithms, particularly matrix factorization. It iteratively updates the user and item factors to minimize a loss function, typically the difference between observed and predicted ratings. It's an efficient way to handle large-scale data and is a key component in many model-based recommendation algorithms.

