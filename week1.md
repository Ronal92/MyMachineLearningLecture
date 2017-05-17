
>>이 강의는 Coursera의 Machine Learning 강의(Andrew Ng 교수) 입니다.
>>주요 내용 정리는 아래 링크를 따라서 개인공부로 정리한 한 겁니다. 자세한 설명은 "Coursera >
>>Machine Learning" 강의나 아래 출처로 들어가면 됩니다.
>>출처 : <https://alexdataclass.wordpress.com/2016/01/15/week01-intrdoction/>

# [Introduction]

## 1. 머신러닝의 필요성

대용량의 데이터를 사람이 분석할 수가 없다. 따라서 기계를 학습시켜서 빅데이터로부터 유의미한 해석을 가져오기 위해 사용하기 시작함.

## 2. Supervised Learning
                            - right answers -
입력에 대한 답이 무엇인지를 알고리즘에 알려주면 기계는 주어진 데이터(입력값, 결과값)로부터 학습을 통해 알고리즘을 만든다.

학습 알고리즘은 크게 Regression Model과 Classification Model 으로 나뉜다.

(1) Regression Model은 연속적인 데이터(continuous input data)를 이용하여 결과를 예측할 수 있다.

(2) classification Model은 입력값이 어떤 분류(discrete output)에 속할 지 확률을 예측하는 것이다.

## 3. Unsupervised Learning
    
Unsupervised Learning은 명확한 정답이 존재하지 않기 때문에 데이터들을 어떻게 clustering 할것인지에 대한 학습이다.

--------------------------------------

# [Linear regression with one Variable]

## 1. Model representation

![](http://cfile8.uf.tistory.com/image/217679425916F5F50BD312)

집의 크기에 따라 가격이 결정되는 그래프입니다. 

 여기서 분홍색 선처럼 정확한 straight function을 구하기 위해서는 Training 집합을 가지고 Learning Algorithm을 통해 h(hypothesis)라는 학습된 가정을 만들어 집의 크기 X(Size)가 들어왔을 때 추정하는 y(Price)값 즉 Price($)를 구해야 합니다.

  hypothesis는 입력값에 대해 출력값을 추론하는 수식입니다. 즉 예상되는 예측값을 출력하는데, 문제는 이 예측값과 실제값이 차이가 Minimize해야 한다.

 이 정확도를 높이기 위해 지속적으로  training set을 learning algorithm을 이용하여 지속적으로 학습함으로써 최적의 h를 찾는 것이 바로 머신러닝이다. 

 ## 2. Cost function

 Cost function의 아이디어는 임의의 straight function과 실제 값들(training 집합)과의 차이가 가장 작은 θ0, θ1을 찾는 것입니다.

 ![](http://cfile2.uf.tistory.com/image/213B404E5916F8431C68C3)

  ▼ Cost Function J(θ0,θ1)의 수식은 아래와 같습니다.

  ![](http://cfile22.uf.tistory.com/image/2353904A5916F79D2B4A64)
