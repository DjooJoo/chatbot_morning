Chatbot_MorningCoffee
=====================
Slack 챗봇 프로젝트
이 게시물은 Samsung Software에서 만든 프로젝트

주제 선정 배경
-------------
- 아침에 간단하게 모닝커피를 한잔 마시며 체크하는 오늘의 이슈, 오늘의 날씨 등을 알아보는 챗봇

요구사항
-------
- 네이버 구미 인동 날씨 사이트를 크롤링하여 제공
- 네이버 뉴스 헤드라인을 크롤링하여 제공
- BUGS 실시간 음악 순위를 크롤링하여 제공
- CGV 영화 예매 순위 사이트를 크롤링하여 제공


내부구조
-------
1. 챗봇 call
![첫페이지](./image/1.png)
- 처음 챗봇을 부르거나, 원하는 단어가 없을 시에 나타나는 텍스트

2. 날씨 정보 call
![날씨](./image/2.png)
- 날씨, weather 의 단어가 들어가는 문장을 입력할 시 '오늘'부터 7일간의 '구미 인동'의 날씨를 알려줌

2-1. 지금 날씨 정보 call
![지금날씨](./image/3.png)
- 지금, now 그리고 날씨, weather의 단어가 들어가는 문장을 입력할 시 현재 '구미 인동'의 날씨를 알려줌
  - 미세먼지의 농도의 나쁨을 기준으로 문장이 변경되어 나옴
  
3. 오늘의 뉴스 call
![뉴스](./image/4.png)
- 이슈, news, 뉴스의 단어가 들어가는 문장을 입력할 시 오늘의 주 topic 뉴스를 10개 보여줌

4. 음악순위 call
![음악](./image/5.png)
- 음악, music의 단어가 들어가는 문장을 입력할 시 실시간 음악 차트 10개를 보여줌

5. 영화순위 call
![영화](./image/6.png)
- 영화, movie의 단어가 들어가는 문장을 입력할 시 실시간 음악 예매 순위 7개를 보여줌

  

개발환경 
-------- 
- FLASK
- Python


모닝커피 한잔과 함께하는 오늘의 이슈, 날씨 등을 알아보는 챗봇
