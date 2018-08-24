https://ratsgo.github.io/machine%20learning/2017/03/26/tree/

<CART>

## 1.classification tree
반응변수가 질적이다(범주형 변주) : 클래스(0 혹은 1)를 나눌 사용. 각 데이터의 클래스 분류를 위해서 사용한다.
오차율 : 각 leaf 안에서 발생하는 잘못된 예측치의 개수/ 잘된 예측치의 개수

분류트리에서는 관측치가 속하는 영역 내에서 훈련 관측치들이 가장 많이 포함된 클래스가 해당 관측치의 클래스로 정의된다. 아래 그림에서는 R(s)에서 빨간 삼각형이 많으므로 이 클래스는 '빨간 삼각형'으로 정해지게 된다.

![](https://user-images.githubusercontent.com/23113869/44577603-82894000-a7cc-11e8-93a0-5d77610d355c.jpeg)

#### classification tree의 분류과정은 아래와 같다.
![](https://user-images.githubusercontent.com/23113869/44577602-82894000-a7cc-11e8-9c1d-f826fc7baf98.png)
    (1) Choose j and s to minimize E(R) : 위 그림에서 s를 기준으로 R의 왼쪽 영역과 오른쪽 영역으로 구분된다. 이 때, 각 영역의 Error값이 작아지도록 j와 s를 결정하라는 말!
    (2) Choose j and s to minimize in R(k) : R(k)는 leaf node이다. leaf node가 나올 때까지 반복해서 j, s를 구하라.
    (3) Terminate when there are only pointes < 5 in a subset or
                  when there are only one class in a subset





장점 : 분석과정이 직관적이고 이해하기 쉽다



## 2.regression tree
![](https://i.stack.imgur.com/SiSOd.png)
반응변수가 양적이다(연속형 변수) : 특정 영역 혹은 그룹으로 나눌 때.

만약 관측치는 50개인데 5개의 그룹으로 나누고자 한다면 조합순열에 의해 2,118,760이라는 어마어마한 경우이 수가 나타남. 
따라서 recursive binary split 방식으로 나눠야 한다.
recursice binary split 방식이란? MSE(min square error)가 최소가 되도록 최적의 split point를 찾는 과정.

문제) x1과 x2를 3개의 그룹으로 나누기 위해 적절한 point t를 찾되 MSE가 최소가 되는 지점을 구하라 : t1, t2
   1. For each variable X(k)
        Find optimal cutoff point s,
            ![](https://user-images.githubusercontent.com/23113869/44571043-a3489a00-a7ba-11e8-97cd-b98ef038c76f.png)
           
   2.     Choose y yielding lowest MSE
   3.     Terminate when MSE-gain becomes too small
            
위 방식이 그룹을 나눌 때, 각 node에서 최소의 MSE를 찾아나가는 과정이기 때문에(optimal process) greed algorithm이라고 한다.(뭔가 Computer Science의 greedy 알고랑 비슷한 느낌.......)

고려해야할 점 : 과적합의 위험성이 존재하기 때문에 Pruning 과정을 거쳐서 의사결정나무를 최적화해야 한다.


<reference>
https://www.youtube.com/watch?v=w4MnOA14pYs

