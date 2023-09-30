---
layout: default
title: 스타트업에서 유저피드백 수용하기-1
parent: PM story-ux, design
nav_order: -3
---




사내의 프로덕트에 대한 사용자의 피드백을 어떻게 구해야 가장 진실된 답변을 얻을 수 있을까 고민인 요즘이다..
처음엔 사용횟수에 따라 누적된 사용량이 일정 횟수에 도달하면 Pop-up survey를 통해 별점을 평가하고 그 후에 부담 없이 의견을 남길 수 있도록 하였다.
하지만 의견을 남기는 텍스트 영역에 스킵 가능이라는 문구가 포함되어서 그런가? 의견 문구를 남겨준 사용자가 거의 0에 수렴했다.
이 프로덕트가 런칭된지 얼마 되지 않았기 때문에, 정량적인 평가보다는 정성적인 평가에 많이 귀기울이고 싶은데, 헤비유저의 자발적 평가를 기대하긴 어려운 것 같다.. ㅠ
어떤 UX Writing을 해야 사용자가 우리의 제품에 대한 솔직한 평가를 남겨줄지 여러 글들을 찾아보며 정리해보는 시간을 가져야겠다.

## Indeed 아티클의 내용 정리

### Ways to ask for feedback from customers

<ul>
  <li>이메일 보내기: 서베이를 포함하여 보내거나, 웹사이트나 다른 데이터 수집 도구로 redirect할 수 있도록</li>
  <li>Pop-up 서베이 사용하기: 사용자가 라이브챗이나 온라인 구매 같은 경험을 한 후 바로 피드백 요구. 별점을 선택하게 할 수도 있고, 높거나 낮은 숫자를 선택하고 코멘트를 더하게 할 수도 있다. 빠르게 의견 수렴 가능.</li>
  <li>소셜미디어에 투표하기: 서비스의 소셜미디어를 통해 피드백 요구하기. 빠르게 투표할 수 있는 방법을 제공하면 편리하게 의견 수렴이 가능.</li>
  <li>웹사이트 혹은 앱에 피드백 혹은 연락하기 넣기: 사용자에게 피드백을 언제든 보낼 수 있는 창구를 제공. 이 방법을 잘 이용하려면, 발견하기 쉽고 완료하기 쉽게 만들어라. CTA(call-to-action) 버튼을 모든 페이지에 더해서 사용자가 언제든 누를 수 있도록 해라. </li>
  <li>서드파티 리뷰 요청하기: CTA 버튼을 통해 사용자가 서드파티 리뷰 사이트나 소셜미디어플랫폼으로 이동하여 리뷰를 남길 수 있도록 할 수 있다. 예)음식점이라면 배민에 리뷰 남기기</li>
  <li>아티클 피드백 요청하기: 만약 사이트나 블로그에 support 글이나 교육적인 글을 기고한다면 "Was this helpful?" 같은 질문과 함께 "Yes" 나 "No"를 통해 의견을 물어볼 수 있다. No를 선택했다면 dialog box가 등장하며 이유를 설명해주도록 할 수 있다.</li>
  <li>문자보내기: 문자를 보내서 피드백을 주도록 요구. 서베이 할 수 있도록 링크를 보낼 수도 소셜미디어 페이지로 가서 리뷰를 남기도록 요구할 수도 있음.</li>
  <li>전화하기: 사내 전화번호를 따로 두고 전화하여 제품이나 서비스에 대한 특정 질문을 할 수 있음. (하지만 나라면 전화 받으면 제품에 대한 평가가 좋지 않아질 것 같음...)</li>
  <li>질문지 메일 보내기: 이메일이 아닌 진짜 물리적 메일로도 할 수 있음.</li>
</ul>

### Questions you should ask your customers to get feedback
사용자 피드백을 요구할 때, open-ended(열린) 질문을 해라.

예시:
<ul>
  <li>How was your experience today?(오늘의 경험은 어떠셨나요?)</li>
  <li>How could this product be better?(이 제품이 어떻게 더 나아질 수 있을까요?)</li>
  <li>What do you think about this product?(이 제품에 대하여 어떻게 생각하시나요?)</li>
  <li>What specific features about this product did you like?(이 제품의 어떤 특정 기능이 마음에 드셨나요?)</li>
  <li>What could have convinced you to purchase the item in your cart?(무엇이 이 아이템을 장바구니에 넣게 만들었나요?)</li>
  <li>What service did we provide for you today?(오늘 어떤 서비스를 제공받으셨나요?)</li>
  <li>Why did you choose us to provide this service?(이 서비스를 이용하기 위해 우리 제품을 선택한 이유가 무엇인가요?)</li>
  <li>How would you rate this product or service?(이 제품이나 서비스를 어떻게 평가하시나요?)</li>
  <li>How could we improve this product or servicd?(이 제품이나 서비스를 어떻게 개선시킬 수 있을까요?)</li>
  <li>How satisfied are you with your product or service?(우리의 제품이나 서비스에 대해 얼마나 만족하셨나요?)</li>
  <li>Would you recommend our product or services to others?(우리의 제품이나 서비스를 다른 사람에게 추천할 의향이 있나요?)</li>
  <li>How did we meet or exceed your expectations? If we didn't, what else could we have done?(우리가 당신의 기대를 충족시켰나요? 그렇지 않다면 우리가 무엇을 할 수 있을까요?)</li>
</ul>

### How to ask for feedback from customers
피드백을 물어보려면 아래의 단계를 따라하라:

<ol>
  <li>Decide which questions to ask: 질문을 하기 전에 비즈니스 차원에서 어떤 것에 집중할 것인지 정하고 그걸 위한 특정한 질문을 해라. 그리고 가장 매력적으로 질문해라.</li>
  <li>Plan your method: 제품이나 서비스를 위해 가장 좋은 방법을 선택해라.</li>
  <li>Make a connection with your customers: 사용자를 개입시키는 가장 좋은 방법은 연락도구가 가장 사람처럼 느껴지게 하는 것이다. <b>피드백을 요구할 때 그 사람의 이름을 불러라.</b> ~~이 방법으로 AB 테스트 해봐야겠다~~ <b>혹은 메일을 끝마칠 때, 특정한 팀 멤버를 넣으며 마무리 지어라</b> 사용자의 의견을 더 잘 수렴하는 방법은 개인적인 연결성을 넣는 것이다.</li>
</ol>

### Tips for asking for customer feecback
더! 잘! 유저피드백을 모으기 위한 몇가지 꿀팁:
<ul>
  <li>열린 질문을 해라</li>
  <li>이메일 피드백 요구라면 제목을 잘 만들어라. ex) 온라인 경험 개선에 도움을 주세요</li>
  <li>피드백이 고맙다는 것을 잘 표현하라. 정말 중요.</li>
  <li>피드백을 준 사용자에게 프로모션 이벤트를 제공하라.</li>
  <li>물어보지 않았는데 피드백을 준 사용자를 찾아라: 어떤 사용자 유형이 이러는지 잘 들여다보고 긍정적 혹은 부정적 경험을 하였나 잘 살펴라.</li>
  <li>부정적 피드백에 반응하여라: 부정적 피드백에 대해 빨리 올바르게 반응하여 브랜드 평판을 개선시킬 수 있다. 문제를 웹사이트에서 공적으로 다룬다면, 다른 사용자도 문제를 해결하려고 노력하고 있다는 것을 알 수 있으니 더 좋음. </li>
  <li>다른 사람들이 남긴 피드백에 투표할 수 있도록 해라: 이를 통해 어떤 사용자 의견이 가장 인기있고 관련있는지 알 수 있다. 오픈피드백 방식.</li>
</ul>



> 참고<br>
> [indeed](https://www.indeed.com/career-advice/career-development/how-to-ask-feedback-from-customers)에서 Ways to ask for feedback from customers만 읽음