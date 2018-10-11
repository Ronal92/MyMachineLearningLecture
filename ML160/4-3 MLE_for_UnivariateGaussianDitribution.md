>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=XtUNwVrWnPM&index=24&list=PLD0F06AA0D2E8FFBA (4.3))

# MLE 구하는 식    
이전 글에서 정리한것처럼 MLE란 현재 우리에게 주어진 증거(표본)를 가지고 모집단의 ‘모수’를 알아내는 것이다.
확률변수들의 모임 :  
![](https://user-images.githubusercontent.com/23113869/46808320-04e2b900-cda7-11e8-85d6-be24fcbdf058.png)

확률밀도함수(or 확률질도함수) : f

가능도 L(θ) 는 

![](https://user-images.githubusercontent.com/23113869/46808322-07451300-cda7-11e8-88cd-9425133bd66e.png)

 이다.

이때, 가능도 함수에 로그 함수를 씌우더라도 원래 구하고자 하는 MLE 값을 구할 수 있기 때문에 최종 식은 아래와 같다.
 
![](https://user-images.githubusercontent.com/23113869/46808324-0ad89a00-cda7-11e8-8c69-d6965484e078.png)

# 최대우도확인법을 통해 모평균 추정하기

 예상 : 표본 (x(1), x(2), ………………, x(n))을 이용했을 때, 모평균의 추정값은 
![](https://user-images.githubusercontent.com/23113869/46808328-0d3af400-cda7-11e8-889b-8aef70af82ba.png)
 이다.

최대우도확인법 : 


  1. 정규분포함수
![](https://user-images.githubusercontent.com/23113869/46808338-11ffa800-cda7-11e8-8880-8b844880162d.png)

                       
  2. 여기에 로그를 씌워주면
![](https://user-images.githubusercontent.com/23113869/46808344-13c96b80-cda7-11e8-9235-68da1a05c5f5.png)

 
      3. 최대우도값을 찾기 위해서는 미분했을 때, 0인 값 즉 극대값을 찾아야 한다.
![](https://user-images.githubusercontent.com/23113869/46808346-162bc580-cda7-11e8-8c95-a998ad601cc8.png)

위 식에 표본 평균으로 편미분하면,
 

4. 최대우도를 찾기위한 모평균의 추정량은 
    
    ![](https://user-images.githubusercontent.com/23113869/46808351-1af07980-cda7-11e8-859a-6c2ad7a50724.png)

           이다. 따라서 우리가 처음 예상한 모평균의 추정량과 같다.
      (  어떻게 보면 맞는 말인 거 같다. 최대우도란 것이 현재 가지고 있는 증거들을 가지고 전체 모수에 가장 근접한 가능성을 지니는 통계량을 추정하는 것이기 때문에 샘플을 통해 표본평균을 구한 값이 전체 모평균의 값을 따를 수 밖에 없지 않을까…… 추측 )



<참고>
https://wikidocs.net/7679

