

4.4 ~ 4.5 MLE for a PMF on a finite set

# MLE를 이용한 통계량 추정법(일반화)

Likelihood를 Bernoulli 분포로 표현하면
 
y(n)은  각 샘플 데이터들의 확률.
t(n)은 Posterior로써 0 or 1 값(Label)

위 식에 Log를 씌우면  아래와 같은 식이 나온다. 우리는 아래 식을 Maximize해야 한다.

 

위 식의 극대값을 찾아야 되므로 미분했을 때, 0이 되는 값을 찾는 방향이 MLE를 구하는 과정이다.


# MLE와 크로스엔트로피 관계 
 크로스 엔트로피를 최소화하는 것이 곧 우도를 최대화하는 것이다.(확률적 의미)
     * 크로스 엔트로피 : 딥러닝에 사용되는 손실함수(loss function)
즉 최대우도추정은 우리가 가진 데이터의 분포와 모델이 학습하여 예측한 데이터 분포 사이의 차이를 줄여주는 ‘모수’를 찾는 과정이다.








### 참고
  (https://taeoh-kim.github.io/blog/cross-entropy%EC%9D%98-%EC%A0%95%ED%99%95%ED%95%9C-%ED%99%95%EB%A5%A0%EC%A0%81-%EC%9D%98%EB%AF%B8/)
(https://ratsgo.github.io/statistics/2017/09/23/MLE/)




