>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=kkhdIriddSI&list=PLD0F06AA0D2E8FFBA&index=31(6.1))


# Maximum a posterior


MLE가 오직 주어진 데이터들만 가지고 parameter를 추정하는 방식. 오직 지금 주어진 데이터만을 잘 설명하는 parameter 값을 찾게 된다. --> overfitting 될 수 있다.


MAP는 여러 parameter들 중에서 데이터가 주어졌을 때, 가장 확률이 높은 θ를 고른다.
   좀더 쉽게 설명하면, MLE는 Likelihood만 고려하여 최적의 Parameter θ를 구하지만, MAP는 Likelihood와 함께 Prior Probability(~ 선입견)를 고려하여 최적의 θ를 구하는 방법이다.
![](https://user-images.githubusercontent.com/23113869/47292330-983aaa80-d641-11e8-80e9-0351696d5f0a.png)

# 예시

문제 : 동전을 던졌을 때, 앞면이 나올 확률이 0.5인가? 우리가 가지고 있는 증거는 동전을 100번 던졌을 떄, 70번이 앞면이 나왔다.


--> MLE  방식 : 앞면이 나올 확률 T를 0.5, 0.6, 0.7 등으로 가정하면서 현재 가지고 있는 증거를 가장 잘 설명하는 값을 최종 확률로 구했음.

하지만 MLE 에서는 동전을 던졌을 때, 앞면이 0.5 라는 우리의 선험적 지식을 활용할 수 없다. 이것을 활용하려면 MAP를 활용해야 한다.

--> MAP는 : 
                P(T|E) = P(E|T)P(T) / P(E) 베이지안으로 구함.

만약 우리의 선험적 지식인 P(T=0.5)으로 계산하면
![](https://user-images.githubusercontent.com/23113869/47293520-57dd2b80-d645-11e8-860e-53d71021f3b6.png) 으로 나온다.

이와 같이 T의 x를 바꿔가면서 우리의 선험적 지식을 활용했을 떄, x의 변화에 따라 P(T|E)를 최대값을 구하는 과정이 MAP 이다.


## 참고
http://arkainoh.blogspot.com/2018/04/parametric.learning.maximum.a.posteriori.estimation.html

http://databaser.net/moniwiki/pds/BayesianStatistic/베이즈_정리와_MLE.pdf