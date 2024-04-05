# 통계학과 자연어처리 PBL
## 우울감정분석

👨‍💻 팀원: 조용진, Xu Zekai <br>
🕑 준비기간: 2022.11.09 ~ 2022.12.21<br>
🖥 분석도구: Python

## 1. 사용 데이터
- 언어: 한국어
- 출처: AI 허브
- 데이터 건수: 46,009

|index|연령|성별|감정\_대분류|감정\_소분류|사람문장|
|---|---|---|---|---|---|
|0|청년|남성|기쁨|신이 난|아내가 드디어 출산하게 되어서 정말 신이 나\.아 지금 정말 신이 나\.|
|1|노년|남성|불안|스트레스 받는|당뇨랑 합병증 때문에 먹어야 할 약이 열 가지가 넘어가니까 스트레스야\.건강할 때 관리 좀 잘할걸 하는 생각이 들더라고\.|
|2|청소년|여성|당황|당황|고등학교에 올라오니 중학교 때보다 수업이 갑자기 어려워져서 당황스러워\.아직 학기 초인데 내가 수업에 잘 따라갈 수 있을지 걱정돼\.|
|3|노년|남성|기쁨|신이 난|재취업이 돼서 받게 된 첫 월급으로 온 가족이 외식을 할 예정이야\. 너무 행복해\.퇴직 후 다시는 돈을 못 벌 줄 알았는데 이렇게 월급으로 가족에게 맛있는 밥을 살 수 있어서 너무 행복해\.|
|4|노년|여성|기쁨|안도|빚을 드디어 다 갚게 되어서 이제야 안도감이 들어\.빚도 다 갚았으니 당분간은 아무 생각도 안 하며 살고 싶어\.|
## 2.분석 목적
```
일상 대화에서 사람들은 얼굴 표정과 말투를 통해 감정을 표현하고 이해합니다.
그러나 SNS나 메시지 같은 문자 기반의 커뮤니케이션에서는 상대방의 표정을 직접 볼 수 없어 감정을 파악하기 어렵습니다.
본 분석의 목표는 기계 학습 방법을 활용하여 우울한 감정을 감성 분석을하고 우울 감정의 유무를 판단하는 것입니다.
```
## 3. 프로젝트 요약
```
- 감정 대화 코퍼스를 이용한 우울한 감정 분석
- 청소년, 청소년, 노인 대상자의 대화 자료를 이용하여 연령별 감정분석을 실시
- 형태소 단위의 문장을 토큰화하여 데이터 전처리 과정에서 용어를 제거
- TF-IDF 방법으로 전처리된 문장을 벡터화하여 데이터를 기반으로 로지스틱회귀, 랜덤포레스트, SVM 모델로 학습
- 새로운 문장의 감정을 예측하기 위한 모델 활용
- 트리 맵과 워드 클라우드의 데이터를 시각화하고 연령대별로 자주 사용되는 단어를 식별
```
