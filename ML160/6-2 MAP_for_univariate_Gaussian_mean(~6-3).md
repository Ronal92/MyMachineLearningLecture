
>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=KogqeZ_88-g&index=32&list=PLD0F06AA0D2E8FFBA (6.2~ 6.3))




# 6.2  MAP for univariate Gaussian mean

## 연속적인 분포 형태인 Gaussian에서 θ parameter를 찾기 위한 과정!

## 증명 식
Given Data, D = (x1,x2,x3, ……., xn)
Suppose θ is a RV ∼N(μ,1).
Random Variable  X1,………Xn  ~ N(θ, σ2) 이고 iid 조건일 때,

![](https://user-images.githubusercontent.com/23113869/48297181-add71d80-e4e5-11e8-814d-e9432994682e.png)



위 식에서 θMAP 를 찾기 위해서는 1차 미분 결과가 0인 값을 찾는다.
![](https://user-images.githubusercontent.com/23113869/48297183-b0397780-e4e5-11e8-9f72-449228f6eb75.png)
여기서 좌변의 log p(D|θ)의 편미분 값은 MLE를 구하는 식에서 나왔던 거다.
      

우변의 log p(θ)의 편미분 값은 
 ![](https://user-images.githubusercontent.com/23113869/48297184-b29bd180-e4e5-11e8-9bf7-5d5f740bd8f6.png)
 ![](https://user-images.githubusercontent.com/23113869/48297185-b4659500-e4e5-11e8-9865-7909105687bb.png)

이렇게 나온다.

최종적으로 위의 두 식의 극대값은 아래와 같이 나온다.
( 미분했을 때, 도함수가 0인 값이 극대값인 이유는 θ 에 대해 한번 더 미분했을 때,
   이계도함수가 -(n/ σ2  + 1) 모양으로 나온다. 
그리고 위 함수 값은 항상 음수이기 때문에 위로 볼록한 형태인 극대값을 포함하게 된다.)
 ![](https://user-images.githubusercontent.com/23113869/48297192-ef67c880-e4e5-11e8-89a2-ecd2da259f35.png)

결국 극대값을 갖기 위한 θ 값은
 ![](https://user-images.githubusercontent.com/23113869/48297193-f1318c00-e4e5-11e8-84da-0b402275a444.png)
이거와 같이 나오게 된다.

# 6.3 Interpretation of MAP as convex combination

## convex combination이란
    어떤 함수 모양의 형태가 오목하게 들어간 부분이나 내부에 구멍이 없는 집합을 의미한다.
어떤 집합이 convex set이라고 말할 수 있으려면 집합에 속한 임의의 두 점으로 선분(line segment)을 만들어서 그 선분이 집합에 포함되는지를 보면 된다.

![](https://user-images.githubusercontent.com/23113869/48297194-f42c7c80-e4e5-11e8-9e00-8f5642a36fe2.png)
 

위 그림에서는 좌변(Sample Mean)과 우변(Prior Covariance)이 combination set 관계이다.
(  n/(n+σ2) + σ2/(n+ σ2) <=1  이다.  )
Sample Mean의 계수와 Prior Covariance의 계수의 합이 1보다 작거나 같음!

![](https://user-images.githubusercontent.com/23113869/48297195-f5f64000-e4e5-11e8-8804-a4ab2b5c7974.png)
 


x̅ 와 μ 를 선분으로 연결했을 때, n의 값에 따라 parameter가 결정되는 구조임.

# 참고

https://cveai.github.io/notes/2018/04/18/mm-ml-6.html
https://wikidocs.net/17413
