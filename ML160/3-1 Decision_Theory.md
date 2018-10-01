>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=KYRAO8f5rXA&list=PLD0F06AA0D2E8FFBA&index=15)
>>ML(3.1)


# Decision Theory

Decision Theory란, classifier를 통해서 어떻게, 잘, 결정을 내릴 수 있는가에 대한 주제이다.

!()[https://user-images.githubusercontent.com/23113869/45304574-5226fd00-b553-11e8-94a1-ac25568cfc60.png]

위 그림을 보면 None, Lung cancer, Breast cancer 각각의 case에 대해 surgery를 했을 때와 하지 않았을 때의 임의의로 준 에러값들이다.

위와 같이 나타난 에러를 줄이는 것이 곧 Decision Theory이다.

그리고 그러한 방법으로 Loss function : L(y,a)을 사용할 것이다.

Loss function은 쉽게 말하면 실제 '결과값'과 '예측값'과의 차이이다.
단순히 0과 1로 표현하는 binray 방법뿐만 아니라 결과값과 예측값의 차이의 제곱 형태 등
여러 가지로 나타날 수 있다.

#### Reference
- https://www.cs.ubc.ca/~murphyk/Teaching/CS340-Fall07/dtheory.pdf
