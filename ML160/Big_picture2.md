
>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=Ih4R42qPRWo&index=20&list=PLD0F06AA0D2E8FFBA)
>>ML(3.6)


# Supervised Learning
   : 확률밀도함수를 미리 정해두고 가중치를 학습한다. 예, Gaussian Distribution
  대개 좌우 대칭인 경우. 


앞에서 배운
![](https://user-images.githubusercontent.com/23113869/45596348-ac154000-b9f5-11e8-916d-c150461ce66b.png)

를 풀기 위한 많은 방법론들이 아래에 나와 있다.

## 1. Exact inference 

   - Multivariate Gaussian(very nice)
   - Conjugate priors
   - Graphical models

  현실세계에서는 가능하지 않다.
  
## 2. Point estimates of θ(simplest)
   - MLE / MAP(Maximum A Posteriori)
   - Optimazation
   - EM(Expectation Maximization)
   - Empirical Bayes
 

## 3. Deterministic Approximation
   - Laplace Approximation
   - Variational methods
   - Expectation Propagation

## 4. Stochastic Approximation
   - MCMC
   - Importance Sampling(Particle filter)
   
    많이 사용되고 쓰기 쉽다는 장점!