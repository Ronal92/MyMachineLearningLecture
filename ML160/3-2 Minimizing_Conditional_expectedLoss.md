>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=NC_cTB1PHyQ&list=PLD0F06AA0D2E8FFBA&index=16)
>>ML(3.2)


# Minimizing conditional expected loss

실제로 오분류(missclassification)를 줄이기 위해서는 아래와 같은 쉽지 않은 조건들이 있다.
     - 입력값 x가 주어졌을 때, L(y,^y(예측값)) 에서 실제값 y를 알 수 없다...
     - L(y,f(x))를 처리하기 위해 f(f(x)=y)가 주어지지만, x,y를 알 수 없다.....


따라서 확률로 접근한다!
하나의 샘플 x가 C(k)가 아닌  C(j)로 선택할 들어가는 비용을 Loss function이라 정의하고 식은 아래와 같다
!()[https://user-images.githubusercontent.com/23113869/45585435-1ad39a00-b91f-11e8-8412-41120629a37f.png"]

위 함수를 최소화 하는 방법은 Loss 함수에 대한 평균값 자체를 최소하하면 된다.
즉 모든 영역 k에 대해서 j 영역을 옮기면서(그래프 : 확률밀도함수) 에러가 최소가 되는 영역을 찾는 것!
p(x,C(k))=p(C(k)|x)p(x)이고 <-- 베이지안 정리.
p(x) 는 클래스마다 동일하다고 생각하고 생략한다.

#### Reference

http://norman3.github.io/prml/docs/chapter01/5