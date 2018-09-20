>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=frbX2JH-_Aw&index=19&list=PLD0F06AA0D2E8FFBA)
>>ML(3.5)


# ML Basic 

ML의 핵심 개념은 Loss Function = E(L(Y,f(X))) 를 최소화하는데 있다.

지금까지의 Loss function과 Decision Theory를 정리하면,

Discriminative : Estimate P(y|x) directly using D(data)

Generative : Estimate P(y, x) using D(data), then recover P(y|x) = P(y,x)/p(x)

일반적으로 Generative가 더 복잡한 모델을 만들 때, 사용된다.

# Core concept

![](https://user-images.githubusercontent.com/23113869/45596348-ac154000-b9f5-11e8-916d-c150461ce66b.png)

머신러닝의 많은 방법들이 위 식에서 출발한다. 하지만 이해를 못함......