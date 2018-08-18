
>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=4ObVzTuFivY&index=6&list=PLD0F06AA0D2E8FFBA)   
Generative vs Discrimitive


Pattern Recognition : classification에 사용되는 모델은 아래 두가지이다.

## 1. Generative
Generative models model the distribution of individual classes
Generative는 데이터를 가지고 학습, 모델을 생성해서 어떠한 문제가 주어졌을 때, 학습한 걸 바탕으로 classify한다.(각 class의 분포에 주목한다.)

P(X,Y)결합확률 분포로부터 어떤 분포 모델이 데이터 분류에 적합한지 측정한 뒤,
확정된 분포 모델로부터 사후확률 P(Y|X)을 구한다.



## 2. Discrimitieve
Discriminative models learn the (hard or soft) boundary between classes
Discrimitive는 데이터의 모델에는 관심이 없다. 데이터 간의 차이만을 가지고 한다.(각 class의 차이에 주목한다.)

 P(Y|X) 조건부 확률 분포에 근거해서 입력값 X에 대한 출력값 Y를 벡터로 표시.
 최종 Y가 0 or 1인 구분선을 만든다.

결국 최종 목적은 위 2가지를 사용해서 데이터의 분류를 위한 decision boundary를 구하는 것!


----------------------------------------------------------------------
### 추가
결합확률분포와 조건부확률분포 및 argmax에 대한 이해

#### 결합확률분포
![](https://mblogthumb-phinf.pstatic.net/MjAxNzA4MjBfMTE0/MDAxNTAzMjM4NjgyNTk2.72QdqluJEZ7D7EEHPafaVrf8yB3EXDlt4lIC7sFj1D4g.ehHRKcFjPETp2OTyoOn2pB8tCeogY8OBex3NR7F3VEcg.PNG.2feelus/스크린샷_2017-08-20_오후_11.17.11.png?type=w2)

#### 조건부확률 분포
![](https://mblogthumb-phinf.pstatic.net/MjAxNzA4MjBfMyAg/MDAxNTAzMjM4NjYyNjYx.aKmZvJ2UwEj56KRqaKKZbaRz0IuzVa6RMfYLPiuXxwsg.ZDey70bHqZq3KyVtnxZUxjAmZRL1cz_Iyb9cGEBvgtMg.PNG.2feelus/스크린샷_2017-08-20_오후_11.17.30.png?type=w2)

위 표에서 보면 X가 1이라는 조건에서 Y가 1일 확률이 가장 높다. 따라서 X가 1이라는 조건이 있다면 우리가 예측할 수 있는 값은 Y=1이라는 사실! 
  argmax(P(Y|=1)) = 1


참조
   https://m.blog.naver.com/PostView.nhn?blogId=2feelus&logNo=221078340870&proxyReferer=https%3A%2F%2Fwww.google.com%2F
