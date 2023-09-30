---
layout: default
title: Product Usage Metric_Feature Usage
parent: PM story-ux, design
nav_order: -23
last_modified_date: 2023-01-08
---
# {{page.title}}
<span style = "color: #A39FAD">Last modified: {{page.last_modified_date}}</span>

> 참고:
> [HockeyStack-Top 6 Product Usage Metrics To Track TODAY](https://hockeystack.com/blog/product-usage-metrics-to-track/)


## 제품 사용도는 왜 중요한가?
1. 더 좋은 사용자 경험을 만들어 낼 수 있다.
2. 리텐션(고객이 돌아오는 정도)을 높일 수 있다.
3. 전환률을 높일 수 있다. (buyer intent data를 통해)
4. 신뢰할 만하다. (정성적 데이터에 비해 객관적)


## 제품 사용도는 어떻게 측정할까?
### 사용시간을 기준으로 사용도 측정하기
제품의 사용시간은 하루/일주일/한달 을 기준으로 측정할 수 있다. 특히 이는 SaaS 제품을 위한 수치에서 긍정적인 신호로 이용할 수 있고, Customer engagement를 암시한다. (\*하지만, 사용시간은 사용성과 반대되는 지표로 작용할 수 있기 때문에 주의해서 살펴봐야 한다.)
(모든 engagement는 positive도 있고 negative도 있다.)

→ 사용시간은 세션이 얼마나 지속되었는지를 확인하면 된다.


### Time to Value(TTV)를 기준으로 사용도 측정하기
TTV는 새로운 고객이 제품의 가치를 얻거나 실현하는 데 걸리는 시간이다. TTV는 제품이 어떤 서비스를 제공하는 지에 따라 다르다. 

**중요한 TTV의 종류**
1. Time to the basic value: 사용자들이 제품에서 최소한의 가치를 얻어내기까지의 시간. (꼭 유료 버전에서만 가능하지 않고 무료 버전이나 시험 버전 때도 최소한의 가치를 경험해 볼 수 있도록 할 수 있다.)
2. Time to exceed the value: 사용자들이 제품의 더 깊은 가치를 알기까지의 시간.
3. Immediate time to value: 사용자들이 제품을 사용을 시작하고 즉각적으로 효과를 얻었을 때. 

TTV가 짧으면 사람들이 만족을 하는 시간이 더 빠르기 때문에 TTV를 줄이는 것은 중요하다. 이는 더 낮은 이탈(churn)으로 이어진다. 하지만 제품에 따라 TTV를 줄이는 것에 대한 한계가 있을 수 있다.

**TTV 계산법**
TTV는 지속적으로 계산해야 하는 수치이다. 단순한 수식은 존재할 수 없다. TTV를 계산하기 위해 중요한 것은 'value'가 무엇인지이다. (ex. 새 기능의 사용 시작, 유료 버전으로의 업그레이드, 그들이 원하는 ROI(Return on Investment) 달성 등) Value를 얻을 수 있는 행동을 정했으면, 사용자들이 이 행동을 하는데까지 걸리는 시간을 측정하면 된다.


### 기능 사용도를 기준으로 제품 사용도 측정하기
기능 사용도(Feature usage metrics)는 제품의 기능에 대한 사용자의 행동과 연결된 지표이다. 기능 사용도를 측정하는 방법은 다양하다.

그 예로는,
- 총 제품 사용자 중 몇 퍼센트가 그 기능을 사용하는지 → 얼마나 많은 사람들이 그 기능을 사용하는지
- 기능을 사용하는 총 사용자 수 → 그 기능을 사용하는 사용자의 절대적인 양
- 각 사용자 별 기능 이용에 대한 평균 시간 (~~the average time between feature usages of each user~~) → 특정 기능을 얼마나 잦은 주기로 사용하는지

**기능 사용도 계산법**
특정 기간 동안 기능이 사용된 총 횟수를 확인하고 그 기능을 사용한 사람 수를 확인하여 일별 평균 사용 수(average use per day)를 계산한다.

Average use per day 계산식 = 하루 동안 기능이 사용된 수 / 하루 동안 기능을 사용한 사람 수

혹은 전체 고유 사용자 중 얼마나 많은 사람들이 사용하는지를 아래와 같은 수식으로도 확인할 수 있다.

Percentage of unique feature users = 기능을 사용하는 고유 사용자 / 총 고유 사용자 x 100


### 활성화율을 기준으로 제품 사용도 측정하기
여기서의 활성화는 AARRR(Acquisition - Activation - Retention - Revenue - Referral)에서의 Activation을 뜻한다. 활성화는 사용자가 제품의 가치를 알고 온보딩 과정에서 주요한 행동을 했을 때를 기준으로 파악이 될 수 있다. (예를 들어, 무료 플랜 사용을 마치고 구독을 시작했을 때)

활성화율은 SaaS 사업에서 가장 주요한 지표중 하나이다. 이를 통해 얼마만큼의 사용자들이 제품을 통해 정말 원하는 가치를 실제로 얻어내는지를 확인할 수 있다.

**활성화율 계산법**

활성화율 계산식 = 활성화 포인트를 달성한 사용자 수 / 회원가입한 사용자 수 x 100

\*Referral과 관련하여 viral coefficient라는 개념도 존재함. 한 명이 한 명을 데려오면 1. 다섯 명이 한 명을 데려오면 .5 → viral coeffieicnt가 1을 넘어가면 대박인 것. (더 검색해보기)

### MRR의 증가를 기준으로 제품 사용도 측정하기
\*MRR = Monthly Recurring Revenue
MRR의 증가란, 기존 고객들이 추가 지불을 하게 되는 경우를 말한다. 그런 경우들의 종류는 아래와 같다.
- Upsells: 상위 플랜 사용 혹은 무료 플랜에서 유료 플랜으로 변경하여 사용
- Cross-sells: 주요 구매에 가치를 더해주는 추가 제품 구매
- Add-ons: 사용자가 현재 구독중인 것의 일부가 아닌 추가적인 기능으로 기존 사용자들만 구매할 수 있는 것
- Reactivation: 구독 취소를 한 사용자의 재사용

Expansion MRR(MRR의 증가)은 더 이상의 사용자 획득 비용(CAC: Customer Acquisition Cost)이 발생하지 않기 때문에 수익을 창출하기 쉽다. 따라서 Expansion Rate(증가율)은 SaaS에서의 주요한 지표 중 하나이다.

**MRR 증가율 계산법**
MRR 증가율 계산식 = 월말 MRR 증가분 - 월초 MRR 증가분 / 월초 MRR 증가분 x 100


### Stickiness를 기준으로 제품 사용도 측정하기
Stickiness는 고객이 제품을 얼마나 오래 지속하여 사용할 것인지를 측정하는 것이다. 그 결과 사용자들은 제품을 지속하여 구매할 것이다. 

높은 Stickiness는 아래의 요소들에 긍정적인 영향을 준다.
- 이탈률 줄이기
- up-sell과 cross-sell 기회 올리기
- LTV(Life time value) 올리기 = CLV(Customer Lifetime Value)
- 사용자의 더 많은 referrals

\*LTV는 CAC에도 영향

**Stickiness 계산법**
Stickiness 계산식 = DAU() / MAU


