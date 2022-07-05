---
published: false
comments: true
categories: "Deep-Learning"
tag: [deep learning, neural network]
toc: true
author_profile: false
---

**[Index]**[딥러닝 로드맵](https://heo-civil.tistory.com)
{: .notice--danger}

{% include video id="C2sqt9pG6K0" provider="youtube" %}

# 딥러닝(Deep Learning)

## 딥러닝 개념
 딥러닝이란 무엇일까요? 딥러닝을 쉽고 정확하게 설명하기 위해 인공지능과 머신러닝이 무엇이고, 딥러닝과 어떤 관계인지부터 설명하겠습니다.
먼저 인공지능은 컴퓨터가 스스로 문제를 인식하고 해결하는 지능을 가지는 것을 의미합니다. 인공지능을 구현하는 여러가지 방법중에 데이터를
스스로 학습하여 지능을 가지는 것을 머신러닝이라고 하며 그 중에서 인공적인 신경망 형태의 기법을 딥러닝이라고 합니다.
 그러면 머신러닝과 딥러닝은 어떻게 다를까요? 딥러닝은 신경망 구조로 인해 더 많은 데이터를 필요하기 때문에 더 복잡한 문제를 풀 수 있고,
한 모델을 상대적으로 더 많은 문제에 적용이 가능하다는 장점을 가지고 있습니다.


## 딥러닝 구조
<img src="../../images/2022-07-04-deeplearning/dnn_archtecture.png" height="300px" width="700px">  

 딥러닝은 인공 신경망의 구조를 가지고 있습니다. 인공 신경망은 크게 입력층, 은닉층, 출력층으로 나뉘고 입력층은 데이터의 feature 들을
 입력받고 은닉층은 여러 계층을 쌓아서 더 복잡한 문제를 풀 수 있도록 도와주며 출력층은 모든 계층을 통과하면서 연산된 결과 값을 출력합니다.
 입력층과 출력층은 각각 1개의 계층으로 구성되고, 은닉층의 계층 개수는 데이터나 상황에 따라 유동적으로 바뀝니다. 각 계층은 노드로 구성되어
 있고 이 노드의 개수 또한 유동적으로 변경이 가능합니다. 각 계층마다 노드들은 fully connected 하게 연결되어 있고 노드는 weight 과
 bias 파라미터들을 기반으로한 선형 연산과 활성함수(activation function) 의 비선형 연산이 이루어집니다.

## 딥러닝 원리
 인공 신경망은 순전파(forward propagation) 과정을 통해 결과 값을 얻고 역전파(backward propagation) 과정을 통해 cost function을
이용하여 예측 값과 실제 값 들의 cost 를 구하고 gradient descent 를 이용하여 학습율(learning rate)를 기반으로 출력 층에서
입력층 방향으로 weight 과 bias 파라미터들을 업데이트합니다. 위와 같이 순전파와 역전파 과정을 반복적으로 시행하면서 cost 값이 optimal  
solution에 도달하는 weight 과 bias 파라미터들을 구하여 모델을 생성하여 새로운 값을 예측하는데 사용합니다.
  
