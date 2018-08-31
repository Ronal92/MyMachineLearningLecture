
>> 이 정리는 mathematicalmonk의 유튜부 강의를 보고 정리하는 글입니다. 개인적인 공부 목적으로 
>> 사용합니다. 
>> 자료출처(https://www.youtube.com/watch?v=JM4Y0B6Ho90&list=PLD0F06AA0D2E8FFBA&index=13)
>>ML(2.7)



# Approaches 

### Majority vote 
  각각의 복원추출된 샘플로부터 각각의 classifier가 생성된다. 새로운 데이터 x가 들어왔을 때, 이 classifier 들이 예측한 값들을 투표방식으로 해서 다수가 된 쪽으로 결정된다. 

### Average estimated probabilities 
   각각의 classifier들을 
# 용어 정리
unbiased estimator : 모집단으로부터 크기가 동일한 표본을 무수히 많이 추출해서 이를 정규분포로 나타냈을 때, 표본에서 구한 추정량의 기대치가 추정하고자 하는 모수와 같은 경우이다.

RV : 확률변수
W : True value
PMF : probability mass function (확률질량함수)
PDF : probability density function (확률밀도함수)