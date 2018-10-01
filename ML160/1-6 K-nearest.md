
>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=4ObVzTuFivY&index=6&list=PLD0F06AA0D2E8FFBA)   
Generative vs Discrimitive


K-nearest algorithm : classification에 사용되는 모델은 아래 두가지이다.

## 1. K-nearest algorithm
비모수적 방식( 모집단의 형태에 관계없이 주어진 데이터에서 직접 확률을 계산하여 통계학적 검정을 하는 분석법)이다. 따라서 전체 데이터를 스캔하고 작업하기 때문에 데이터 양이 많을수록 분류할 떄 오래 걸린다.

방법 : 새로운 데이터(2차원 좌표상에서 임의의 한점)가 주어졌을 때, 가장 가까운 k개 이웃의 정보로부터 새로운 데이터를 예측한다.

예시 : 유클리디안 방식으로 접근했을 때, k=1이면 현재 point에서 가장 거리가 가까운 한 점과 같은 속성으로 분류됨. k=3이면 현재 point에서 가까운 3점을 기준으로 분류됨. 



------------------------------------------------------------------


참조
   https://ratsgo.github.io/machine%20learning/2017/04/17/KNN/
