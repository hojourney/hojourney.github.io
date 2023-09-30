---
layout: default
title: Designing Interactive Machine Learning
parent: Papers
nav_order: -26
---


# Interactive Machine Learning (IML) 설계하기 (feat. User Interface Design)




## Machine Learning
우선 인터랙티브 머신러닝을 이야기 하기 전에 머신러닝을 이야기하고 넘어가려고 한다. 머신러닝이라는 단어는 많은 사람들이 들어봤겠지만, 인간이 '학습'을 한다는 것을 모방하여 컴퓨터의 훈련에 적용시킨 개념이다. 일반적으로는, 알고리즘이 어떤 개념을 인식하거나 나타내기 위해서 그 개념의 샘플에 여러번 노출되는 방식으로 학습한다.

하지만, 머신러닝의 성황에도 아직 그 사용법이 어려워 전문 숙련자에게만 좋은 도구로 사용되고 있었던 문제가 존재한다.

이런 문제를 해결하기 위해 등장한것이 IML(Interactive machine learning)이다.
인터랙티브 머신러닝을 통해 비전문가인 사용자도 원래는 다소 다루기 어려운 데이터셋을 자신의 도메인 지식과 통찰을 사용하여 흥미 패턴을 찾거나 복잡한 데이터 드리븐 앱을 발전 시킬 수 있다. 이는 본능적으로 co-adaptive(서로 적응해야 하는)하며 사용자와 기계 사이의 상호작용을 섬세하게 조작함으로써 가능하게 할 수 있다. 따라서 유저인터페이스가 그 중심에 놓여있다.

아직 그 완전한 기본 원리는 부족하지만, 몇 가지 사례를 살펴봄으로써 Interactive Machine Learing에 대하여 정리해보고자 한다.



## IML의 기본적 방법
> The IML process involves the user in the training process by, at the simplest level, using human input in the example selection, creation, and labelling process (Dudley & Kristensson, 2018)

결국엔 Human input를 예시 선택, 생성, 라벨링 과정에 사용하여 사용자를 training process에 개입시킨다는 것이다.  



> Reference: Dudley, J. J., & Kristensson, P. O. (2018). A review of user interface design for interactive machine learning. _ACM Transactions on Interactive Intelligent Systems (TiiS)_, _8_(2), 1-37.