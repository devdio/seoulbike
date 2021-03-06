# seoulbike / 따세권 EDA
[따세권EDA 분석코드 바로보기 ](http://nbviewer.jupyter.org/gist/miningful/42aaa00b607f0fa583ccfcd94475b6eb)

## 따세권이란?
+ 서울시 공공자전거 따릉이 이용이 활성화 되면서 따릉이 대여소 설치 유무에 따라 '따릉이 세권'(따세권)이라는 개념까지 생겨나 비따세권 이용자들의 소외가 우려된다는 언론 보도가 이어짐
+ 실제 따세권이 형성되어 있는지 따릉이 대여소 위치와 대여소별 거치대 갯수 및 이용자 이용현황 등을 바탕으로 분석

## 분석 Flow
### 1.구별 거치대 분포 현황 (구별 거치대 설치 비율이 편향되지 않은지)
+ result1: 영등포-마포구, 강남-서초구에 편향됨을 알 수 있음

### 2.구별 거치대 위치 현황 ( 따릉이 정류소는 대중교통과 인접성을 고려한다는 입지요소 확인)
+ result2: 대부분 도로를 따라 위치하며, 버스정류장과 지하철 역 인접권에 위치한다

### 3.구별 거치대 설치 대수 대비 거치대 이용건수 시각화 (수요와 공급이 불균형 한 지역구가 있는지 확인)
+ result3 : 거치대가 많고 이용건수도 많은 지역 : 마포구, 영등포구(따세권) / 거치대가 많고 이용건수가 적은 지역 : 서초구, 강남구(따세권) / 거치대가 적고 이용건수가 많은 지역 : 중구,동작구,용산구(비따세권) / 거치대가 적고 이용건수도 적은 지역 : 강북구,도봉구,금천구(비따세권)

### 4.따세권으로 자리잡은 지역과 비따세권 지역 대여횟수와 반납횟수 비율(이용 형태 확인)
+ result4 : 거치대가 적고 이용건수도 적은 도봉구,강북구는 반납건수>대여건수 로 반납의 용도로 많이 사용한는 것을 알 수 있음 / 영등포구와 마포구는 반납과 대여가 비슷하게 발생함 / 반면 강남구와 서초구는 반납건수<대여건수로 대여의 용도로 많이 사용하는 것을 알 수 있음

### 5.주간인구지수와 따릉이 이용형태의 연관성(거주인구와 유동인구)
+ result5 : 거치대가 적고 이용건수도 적은 도봉구,강북구는 반납건수>대여건수 로 반납의 용도로 많이 사용한는 것을 알 수 있음(상주인구가 많은 지역은 따릉이 거치대를 반납의 이용으로 많이 이용한다)

### 6.직장인 상권과 관련이 있을까?
+ result6: 따릉이 이용이 유동인구(통근)와 연관성 있는 것은 맞지만 아직 직장인 상권과는 크게 연관성 있어 보이지 않는다.

> 데이터 출처 : 공공데이터 포털(공공자전거,상권데이터,인구데이터)
