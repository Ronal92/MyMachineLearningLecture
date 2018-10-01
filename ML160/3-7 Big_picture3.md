>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=frbX2JH-_Aw&index=19&list=PLD0F06AA0D2E8FFBA)
>>ML(3.5)
>> 주 참고 자료 : (https://cveai.github.io/notes/2018/03/27/mm-ml-3.html)


# Unsupervised Learning
  : 확률밀도함수가 정해져 있지 않기 때문에 사전 지식없이 데이터를 통해서 확률밀도함수를 추정한다.

## Density Estimation
   - 개념 : (관측된) 데이터들의 분포로부터 원래 변수의 (확률) 분포 특성을 추정하고자 하는 것.   
   ![](https://user-images.githubusercontent.com/23113869/45927587-6e259800-bf70-11e8-8d64-250205880a71.png")
  
   히스토그램과 커널함수(KDE)로 나타내는 방식이있다.
   히스토그램은 그리기 쉬우나 관측 step 경계면에서 불연속적이며 관측 step 크기에 따라 관측 시작점과 분포가 달라지는 문제가 발생한다.

   반대로 커널밀도추정은 커널함수를 사용하는 것
   ![](https://user-images.githubusercontent.com/23113869/45927629-1176ad00-bf71-11e8-981d-23bba708ec5b.png)

   히스토그램을 커널함수를 사용하여 나타낸 그림이다.

## 수식

![](https://user-images.githubusercontent.com/23113869/45927663-661a2800-bf71-11e8-9834-000dcd8d0c06.png)





#### 용어 정리 
커널 함수란,  원점을 중심으로 대칭이며 적분값이 1 인 양의 함수로 정의할 수 있습니