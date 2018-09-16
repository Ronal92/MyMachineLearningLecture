>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=AihhnWyl-J0&list=PLD0F06AA0D2E8FFBA&index=18)
>>ML(3.4)


지금까지 classification의 expectation loss를 줄이기 위한 방법을 봤다면
오늘은 regression의 expectation loss를 줄이는 방법을 볼 것이다.

# Square Loss

들어가기 전 전제는, loss function을 square loss로 정의하고 시작한다!

L(y,y^) = (y-y^)^2  일 때,

최소화하고자 하는 loss function의 expectation은 아래와 같다.

![](https://user-images.githubusercontent.com/23113869/45594987-2e463a00-b9df-11e8-90ca-a51ed3c7f879.png)

우리는 최소값을 찾기 위해 미분했을 때, 0인값을 찾으면 된다.(편미분)
자세한 수식 설명은 아래 링크 참조
(https://cveai.github.io/notes/2018/03/27/mm-ml-3.html)

정리 : 결국 loss function이 최소가 되는 지점은 
         y^ = E(Y|X=x) 가 되는 지점이다.
