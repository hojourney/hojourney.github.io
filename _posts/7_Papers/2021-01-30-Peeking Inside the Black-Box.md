---
layout: default
title: Peeking Inside the Black-Box
parent: Papers
nav_order: -1
---


## 간략한 요약

이 글은 개요에서 AI 시대가 다가옴에 따른 XAI의 도래에 대해 말하며 현재까지 연구된 것들에 대한 종합적인 정리를 하겠다고 서술합니다. 도입부에서는 XAI가 필요하게 된 배경에 대한 설명과 XAI의 전망, 활용범위에 대해 설명하며 글을 시작합니다. 또한 글에서 배경과 최근 진행 상황, 네가지 관점에서 본 서베이 형식의 접근, 그리고 앞으로 연구되어야 할 방향과 논의점에 대하여 설명하고 글을 마무리지었다고 서술합니다.

  

## 상세한 정리

### XAI: Explainable AI 
AI가 사회에서 중요한 영향을 가지고 있습니다. 그에 따른 XAI의 도래가 필요하게 되었는데, 그 이유는 AI 알고리즘이 투명성(opacity)에 문제가 있기 때문입니다. AI의 알고리즘은 결과만으로는 내부 구조를 알 수 없고 따라서 왜 그런 결과가 도출되었는지 알 수 없습니다. 이런 것을 표현하기 위한 단어가 Black-box problem 입니다. 결과가 어떻게 도출이 됐는지 표현하기 어려우면 Black box, 잘 표현하면 White box, 중간단계는 Gray box로 표기하기도 합니다. AI의 설명정도를 표현하는 단어로는 Explainability도 있지만 Interpretability도 있습니다. ML(Machine Learning) Community에서는 Interpretability라고 지칭합니다. <br>
XAI(Interpretability)는 AI의 설명가능함을 뜻하지만, 이는 AI의 원리에 있어서 Tradeoff 가 발생합니다. 왜냐하면 정확함(Accuracy)는 데이터의 질(Quality), 양(Quantity)과 관계가 있기 때문입니다. <br>
→ Accuracy(Quality&Quantity) ≠ Interpretability 내 추측: 설명가능하려면 그 구조가 복잡하지 않아야하는데, 원칙적으로 질 높은 데이터를 많이 모아야 Machine Leaning이 가능하기 때문인 것 같습니다. 

### XAI와 관련된 용어
1. **Interpretability = Explainability** (= Understandability = Comprehensibility = Intelligible AI)<br>
   \: Interpretability와 Explainability는 많이 사용되나, Understandability, Comprehensibility, Intelligible AI는 집약적인 단어이고 상황에 따른 변수에서 나온 단어입니다. 
2. **AGI(Artificial General Intelligence)**<br>
   \: AI 영역의 최종 목표, Strong AI, Full AI라고도 표현하며, 인간이 할 수 있는 모든 지능적 업무를 할 수 있는 AI.  
3. **ASI(Artificial Superintelligence)** = 인간을 뛰어넘는 수준의 AI<br>
   
   
### XAI 가 필요한 이유
1. 결과를 정당화하기 위해(Fair, Ethical): AI가 내놓은 결과가 편향되거나 차별적일 수도 있음 ex.인종차별적으로 결과를 내놓지 않았는데, 사용자가 인종차별이라고 할 수 있음. + 법적인 권리로도 설명해야할 이유 있음 
2. 제대로 다루기 위해: 약점이나 결점을 미리 알고 그 기능이 잘못되지 않도록 쓸 수 있음. 
3. 개선시키기 위해: AI에 문제가 있을 경우 발견하고 개선 ex.헤이카카오 가 잘못 대답했는데, 이게 왜 이렇게 대답했는지 알 수 있으면 고칠 수 있음 4. 발견하기 위해: 추후에는 AI를 이용해서 더 심화된 것을 배울 수 있음 ex.알파고를 통해 바둑 승리하는 법 전략 배우기



### 그렇다면 XAI는 언제 필요한가
설명가능한 인공지능 알고리즘을 만드려면 효율이 떨어집니다. 왜냐하면 많은 데이터에 왜를 집어넣기 위해서는 한계가 있기 때문입니다. 그렇기 때문에 XAI가 필요한지의 척도에는 2가지가 있는데, 
1. The degree of functional opacity caused by the complexity of AI algorithm.<br>→ 알고리즘이 복잡한지에 따라 기능적 투명도가 정해지는데, 투명하다면 High level of Interpretability가 필요하지 않음 
2. The degree of resistance of the application domain to errors. <br>→ 에러에 대한 저항도가 높은지. 에러에 대해 저항할 수 있음이 높다면, 에러가 있어도 됨. <br>ex.타겟팅 광고에서 내가 잘못 타겟팅 되어도 무시할 수 있음. 하지만 AI를 이용한 진단이 잘못되었다면 그 에러를 무시할 수 없음. <br>⇒ 이에 따라 XAI가 이용될 수 있는 산업 분야: Transportation, Healthcare, Legal, Finance, Military + Cybersecurity, Education, Entertainment, Government, Image recognition etc. 

### XAI 적용의 한계
- 정확한 AI/ML 모델은 대게 설명하기 어려움: Deep neural nets, Boosted trees, Random forest, Support vector machines 
- 설명가능한 모델은 대게 정확성이 떨어짐: Linear regression, Logistic Regression



즉, 따라서 Accuracy와 Interpretability를 함께 가져가는 것이 XAI의 주된 방향성입니다.




> Reference<br>
> Adadi, A., & Berrada, M. (2018). Peeking inside the black-box: a survey on explainable artificial intelligence (XAI). _IEEE access_, _6_, 52138-52160.