

>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=4ObVzTuFivY&index=6&list=PLD0F06AA0D2E8FFBA)   
Generative vs Discrimitive
>>ML(2.5)


# Generalizations

CART에서 목적은 관측치를 분할할 때, 분할 과정에서 발생하는 정보 이득을 최대화 하는 것입니다.
아래 식 IG는 정보이득(information gain)입니다.
![](https://user-images.githubusercontent.com/23113869/44581871-6e4c3f80-a7da-11e8-83f3-77b8c516e763.png)

I(D(p)) : 부모의 정보이득.
I(D(left)) : 왼쪽 자식의 정보이득.
I(D(right)) : 오른쪽 자식의 정보이득
N : 샘플 노드의 개수

![](https://user-images.githubusercontent.com/23113869/44581925-a5225580-a7da-11e8-94e3-bc9d83d1072e.jpg)



P(i|t) 는 특정 노드 t에서 i 관측치가 c에 속할 확률이다.

## 1. Impurity measures(Classification Error)

## 2. Entropy

## 3. Gini


직접 수식으로 이해하기 위한 참고자료
https://tensorflow.blog/tag/지니-불순도/