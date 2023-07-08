# MiniProject_1

### 서울시 공유자전거 "따릉이"의 수요 예측
#### 날씨요소와 따릉이 수요의 관련있는지 데이터 분석

### 데이터 소개
#### sbikedata.csv

### 데이터 변수 소개
* date : 날짜
* hour : 시간
* temperature : 온도
* precipitation : 강우 여부, 비가 오지 않았으면 0, 비가 오면 1
* windspeed : 풍속(평균)
* humidity : 습도
* visibility : 시정(視程), 시계(視界)(특정 기상 상태에 따른 가시성을 의미)
* ozone : 오존 수치
* PM10 : 미세먼지 수치(머리카락 굵기의 1/5에서 1/7 크기의 미세먼지)
* PM2.5 : 초미세먼지 수치(머리카락 굵기의 1/20에서 1/30 크기의 미세먼지)
* count : 시간에 따른 따릉이 대여 수

### 수치형 데이터와 범주형 데이터로 분할
* 수치형데이터: hour, ozone, temperature, windspeed, humidity, visibility, count
* 범주형데이터: PM10, PM2.5, precipitation, season
* 날짜형 데이터: date, month

- 특이사항: hour를 살펴보니, 오전10시-오후3시에 시간 당 자전거 사용 대수가 높은 것을 활용해 다음과 같이 데이터를
          나눠서 살펴보는 작업을 거침
- 출근 시간대: 오전7시 -오전9시
- 주활동시간대: 오전10시 - 오후3시
- 퇴근시간대: 오후6시 - 오후8시
