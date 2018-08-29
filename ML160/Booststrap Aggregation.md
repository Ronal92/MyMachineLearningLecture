>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=4ObVzTuFivY&index=6&list=PLD0F06AA0D2E8FFBA)   
Generative vs Discrimitive
>>ML(2.6)

# Booststrap Aggregation

- 통계학에서의 의미 : 이는 가설 검증(test)을 하거나 메트릭(metric)을 계산하기 전에 random sampling을 적용하는 방법을 일컫는다.

- ML에서의 의미 : 랜덤 샘플링을 통해 training data를 늘리는 방법

# <Bias / Variance Tradeoff>

### Ensemble methods that minimize variance
   - Bagging
   - Randomg Forests
### Ensemble methos that minimize bias
    - Function Gradient Descent
    - Boosting
    - Ensemble Selection

# 배깅의 목적

– 예측 모형의 변동성이 큰 경우 예측 모형의 변동성을 감소시키기 위해 사용함. 즉, 원자료로부터 여러 번의 복원 샘플링을 통해 예측 모형의 분산을 줄여줌으로서 예측력을 향상 시킴.
– 따라서, 배깅은 일반적으로 과대적합된 모형, 편의가 작고 분산이 큰 모형에 사용하는 것이 적합함.


# 배깅 방법
 1. 주어진 데이터에서 여러 개의 boostrap을 생성한다.(복원추출하여 raw data로부터 크기가 동일하 ㄴ여러 개의 표본 자료를 생성함)
 2. 위에서 생성한 각 자료를 모델링 후, 결합.
 3. 결합 방법은 연속형 변수이면 평균으로, 범주형일 때는 다중 투표(majority vote로)

![](https://swalloow.github.io/assets/images/boosting.png)

# <Bias / Variance Tradeoff에 따른 error>
![](https://user-images.githubusercontent.com/23113869/44790083-4ba29800-abd9-11e8-80b8-d6cc432a4fee.png)

위 수식에 따르면 랜덤 샘플림이 많을수록 좌측의 variance는 줄어들고 우측의 bias는 약간(소폭) 증가하게 된다.

<Reference>
https://learningcarrot.wordpress.com/2015/11/12/부트스트랩에-대하여-bootstrapping/
https://www.slideshare.net/hustwj/an-introduction-to-ensemble-methodsboosting-bagging-random-forests-and-more