
Generative vs Discrimitive

Pattern Recognition : classification에 사용되는 모델은 아래 두가지이다.


1. Generative
Generative models model the distribution of individual classes
Generative는 데이터를 가지고 학습, 모델을 생성해서 어떠한 문제가 주어졌을 때, 학습한 걸 바탕으로 classify한다.(각 class의 분포에 주목한다.)

P(X,Y)결합확률 분포로부터 어떤 분포 모델이 데이터 분류에 적합한지 측정한 뒤,
확정된 분포 모델로부터 사후확률 P(Y|X)을 구한다.



2. Discrimitieve
Discriminative models learn the (hard or soft) boundary between classes
Discrimitive는 데이터의 모델에는 관심이 없다. 데이터 간의 차이만을 가지고 한다.(각 class의 차이에 주목한다.)

 P(Y|X) 조건부 확률 분포에 근거해서 입력값 X에 대한 출력값 Y를 벡터로 표시.
 최종 Y가 0 or 1인 구분선을 만든다.

결국 최종 목적은 위 2가지를 사용해서 데이터의 분류를 위한 decision boundary를 구하는 것!

도움되는 글
   https://m.blog.naver.com/PostView.nhn?blogId=2feelus&logNo=221078340870&proxyReferer=https%3A%2F%2Fwww.google.com%2F