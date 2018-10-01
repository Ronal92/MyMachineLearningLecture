
>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=o7iDkcpOr_g&list=PLD0F06AA0D2E8FFBA&index=14)
>>ML(2.8)



# Random Forests
bagging 알고리즘을 decision tree에 사용한 것.
즉 input 값 x가 주어졌을 때, 여러개의 classifier(tree)로부터 나온 결과를 바탕으로
다수의 의한 투표(for classification)나  average(regression)을 추출한다.


# 과정

  (1) Total set : D 로부터 bootstrap sample D(i........n)를 추출한다.
  (2) 추출한 각각의 D(i........n)로부터 Tree T(i........n)를 구성한다.
  (3) Tree T(i........n)의 각각의 node에서는 m feature 개의 random subspace를 선택하고 이 m feature만을 splitting한다. 

# 용어 정리

- Bias와 Variance는 학습 오류(Learning Error)를 구성하는 두 요소인데 Bias가 높으면 예측결과가 실제결과와 비교해서 부정확한 것이고 Variance가 높으면 예측결과가 어떤 dataset(training set)에서는 엄청 잘 맞다가 다른 dataset에서는 크게 안 맞고 이렇게 예측결과의 안정성이 떨어지는 것(낮은 stability or overfitting)경우이다.

- Bias-Variance Trade Off란 기계학습 알고리즘에서 Bias를 줄이면 Variance가 높아지고 하듯이 두가지 Learning Error들이 일종의 Zero Sum 게임 양상을 보이는 경향인데 Bias-Variance를 극복하는 방법이 Bagging이라는 것이다.

- Bagging은 Bootstrap Aggregation의 약자인데 주어진 데이터(training set)에서 랜덤하게 subset을 N번 sampling해서 (좀 더 정확하게는 observations과 features들을 random하게 sampling) N개의 예측모형을 만들어 개별 예측모형이 voting하는 방식으로 예측결과를 결정하여 Low Bias는 유지하고 High Variance는 줄이는 방법이다. bias-variance trade off를 극복하기 위해 사용되는 방법이다.

(출처 : http://blog.heartcount.io/random-forest-ver-10)