---
layout: post
title: "모각코 3회차"
---
### 목표 : Autograd 패키지로 학습하기

- - -
#### -Autograd 패키지
######  역전파(backprop)를 위해, Tensor의 모든 연산에 대해 미분 값을 자동으로 계산하는 기능을 제공한다. 자동계산을 위해서 사용하는 변수는 torch.autograd에 있는 Variable이다.

###### Autograd 구현에 있어 Tensor 클래스와 Function 클래스가 중요하게 사용되고, 이와 관련된 내용은 학습한 자료에 정리하였다.

#### -Autograd 패키지 학습 내용
###### Jupyter Notebook으로 학습한 파일 '_Project_Mogakko'에 'Autograd 패키지로 신경망 학습하기'로 올려놓았다.
[Github Link](https://github.com/OMEGA-Y/OMEGA-Y.github.io)
- - -

### 결과 
##### Autograd를 구현하기 위해 필요한 클래스들에 대해 학습하였고, Autograd를 활용하여 역전파(backprop)를 해보았다.