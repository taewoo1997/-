# 포트폴리오 프로젝트 소개
개인 프로젝트를 소개합니다.
- [**vision 북체커**](#1-vision-북체커)
- [**딥러닝 모델 기반 실시간 전신주 균열 탐지 및 통합관리 애플리케이션**](#2-딥러닝-모델-기반-실시간-전신주-균열-탐지-통합관리-애플리케이션)
- [**공포 이야기 게시판**](#3-공포-이야기-게시판)
  
# 1. vision 북체커
![vision북체커_안드로이드_4_resize](https://github.com/taewoo1997/Portfolio/assets/108257288/583cd354-6abe-4a94-b338-72ce7c6795d2)
![vision북체커_안드로이드_5_resize](https://github.com/taewoo1997/Portfolio/assets/108257288/1900933e-609f-43d6-9568-360ab59e291e)
![vision북체커_안드로이드_1_resize](https://github.com/taewoo1997/Portfolio/assets/108257288/f0cb2770-7206-491f-863f-681616d9f6f2)
![vision북체커_안드로이드_2_resize](https://github.com/taewoo1997/Portfolio/assets/108257288/ac8ac6bc-0244-4bb9-8698-a59da8710ca7)
![vision북체커_안드로이드_3_resize](https://github.com/taewoo1997/Portfolio/assets/108257288/0ae661a3-abc1-4fc9-98ca-43791b23a390)


## 서비스 내용

도서관 서가 배열 순서 확인 애플리케이션. 도서관에서 책이 순서에 맞게 배열이 되어있는지 확인할 수 있. 스마트폰 카메라를 이용하여, 청구기호가 화면에 들어오도록 동영상 녹화를 진행한다. 동영상 녹화는 책장의 1줄(1칸) 단위로 진행하며 녹화된 동영상을 분석하여 순서가 잘못 되어 있는 책을 발견해낸다.

## 개발 기간
2022.03.03~2022.11.02

## 기술 및 도구
- 언어: Java, Python
- 데이터베이스: SQLite
- 웹 프레임워크: Flask
- 딥러닝 모델: YOLO v5 (Colab을 활용한 모델 학습)
- OCR 서비스: 네이버 CLOVA OCR API
- 이미지 및 비디오 처리 라이브러리: OpenCV
- 이미지 업로드 및 저장: Werkzeug (secure_filename 활용)
- API 통신: Retrofit2 (안드로이드 앱과의 통신)
- 클라우드 플랫폼: OCI(Oracle Cloud Infrastructure)

## 개발 내용

이 섹션에서는 프로젝트의 세 번째 기능에 대한 설명을 작성합니다.

## 기능 분해도
![업무기능 분해도](https://github.com/taewoo1997/Portfolio/assets/108257288/b55a8e5f-39cf-411e-977f-7fff108d6730)

## ERD
![ERD](https://github.com/taewoo1997/Portfolio/assets/108257288/bda7b2d1-ab01-42d1-9838-3e9476ffc28b)
![ERD2](https://github.com/taewoo1997/Portfolio/assets/108257288/6b17240c-0ea5-418b-ab6c-ec4efb7a7d72)


## OCR API 리턴값

![청구기호1](https://github.com/taewoo1997/Portfolio/assets/108257288/1691dab8-1ac1-44bb-b1f6-0474a2d338c0)
![청구기호1_OCR](https://github.com/taewoo1997/Portfolio/assets/108257288/be91c440-bf67-4224-941f-dd1114564467)

## 서비스 데모

![객체탐지](https://github.com/taewoo1997/Portfolio/assets/108257288/b90f4e01-395a-4190-b52c-453c6fa59cb7)

프로젝트의 데모를 보여주는 GIF 파일과 간단한 설명을 작성합니다.

## 모델 성능 평가 지표
![모델처리과정](https://github.com/taewoo1997/Portfolio/assets/108257288/7cb2996c-0a99-4a25-9746-71011b39fc12)<br>
![mAP](https://github.com/taewoo1997/Portfolio/assets/108257288/80d5f5f0-17aa-40a7-af9a-0785801c7688)

## 시연 영상

[![vision북체커 전체](http://img.youtube.com/vi/-kB-40hoIMY/0.jpg)](https://youtu.be/-kB-40hoIMY)


>
> 

# 2. 딥러닝 모델 기반 실시간 전신주 균열 탐지 <br>통합관리 애플리케이션
![크랙터 로고](https://github.com/taewoo1997/Portfolio/assets/108257288/6228700d-a3e9-47f3-9bcf-bca98145344e)
<br>크랙터 = CRACK + DETECTOR 

딥러닝 기반 드론을 활용한 전신주 균열 탐지 + 전신주 현황 통합관리 시스



## 프로젝트 개요

본 프로젝트는 드론을 활용하여 전신주 균열을 탐지하고, 안전 점검을 수행하는 시스템을 개발하는 것을 목표로 했습니다. 
프로젝트 팀은 6명으로 구성되었으며, 저는 주로 안드로이드 앱과 백엔드 시스템 간의 데이터 통신 및 서버 구축을 담당하였습니다.

## 역할 및 주요 기능

- 안드로이드 앱과 백엔드 서버 간의 통신 기능 구현 (Retrofit2 사용)
- 데이터베이스용 백엔드 서버 구축
- 이미지 업로드, 저장 및 관리
- 전신주 정보 및 상태 관리 (MySQL 데이터베이스 사용)
- API 개발 및 관리

## 기술 및 도구

- 언어: JavaScript (Node.js)
- 데이터베이스: MySQL
- 웹 프레임워크: Express.js
- 이미지 업로드 및 저장: Multer
- API 통신: Retrofit2 (안드로이드 앱과의 통신)
- 버전 관리: Git
- 클라우드 플랫폼: OCI(Oracle Cloud Infrastructure)

## API 

1. 전신주 정보 전체 조회
```javascript
app.get('/get', function(request, response) {
    // 데이터베이스에서 전신주 정보를 조회하는 쿼리 실행
    // 결과를 JSON 형식으로 반환
});
```
2. 전신주 1개 정보 조회
```javascript
app.get('/getOne/:id', function(request, response) {
    // 전달받은 ID를 기반으로 특정 전신주 정보를 조회하는 쿼리 실행
    // 결과를 JSON 형식으로 반환
});
```
3. 전신주 이미지 서버로 전송
```javascript
app.post('/postImg/:id', function(request, response) {
    // 이미지 업로드 및 데이터베이스에 저장
    // 업로드 결과를 응답으로 반환
});
```
4. 전신주 이미지 클라이언트에서 조회
```javascript
app.get('/getImgUrl/:id', function(request, response) {
    // 특정 전신주에 대한 이미지 URL 조회
    // 결과를 JSON 형식으로 반환
});
```
5. 전신주 상태 변경
```javascript
app.get('/change_state/:id/:state', function(request, response) {
    // 전신주 상태 변경을 위한 쿼리 실행
    // 변경 결과를 응답으로 반환
});
```
6. 상태별 전신주 정보 조회
```javascript
app.get('/getInfoCheckList/:state', function(request, response) {
    // 상태별 전신주 정보 및 최신 점검일자 리스트 조회 쿼리 실행
    client.query('SELECT utilitypole.utilityPole_id, utilitypole.addr, iu.created_date FROM utilitypole JOIN ( SELECT utilitypole.utilityPole_id, utilitypole.addr, max(img_urls.created_date) as created_date FROM utilitypole JOIN img_urls group by utilitypole.utilityPole_id) as iu ON utilitypole.utilityPole_id = iu.utilityPole_id where utilitypole.state = ? order by created_date desc;' , request.params.state ,function(error, result) {
    // 결과를 JSON 형식으로 반환
});
```

## 특징
- 안드로이드 앱과 백엔드 서버 간 안정적이고 효율적인 데이터 통신 구현
- 이미지 업로드 및 저장을 효과적으로 관리하여 실제 이미지 파일 저장소에 저장
- 데이터베이스를 사용하여 전신주 정보 및 상태를 관리하고 안정적으로 변경
- API를 통해 전신주 정보를 조회 및 변경
- 클라우드 환경에서 백엔드 서버 운영


## 서비스 데모
![ezgif com-resize (2)](https://github.com/taewoo1997/Portfolio/assets/108257288/f4ad1005-8aae-436e-82db-a9c1c205c77a)
![ezgif com-resize (1)](https://github.com/taewoo1997/Portfolio/assets/108257288/0db5a176-8644-4737-a966-08f9a33ad3d6)
![ezgif com-resize](https://github.com/taewoo1997/Portfolio/assets/108257288/5e29156c-a2bc-41bd-8ad2-af96c6cb0e82)


프로젝트의 데모를 보여주는 GIF 파일과 간단한 설명을 작성합니다.



## 모델 적용 이미지
![그림2](https://github.com/taewoo1997/Portfolio/assets/108257288/131a970c-e456-4d1f-8827-d7d2a4cf30c5)
![그림1](https://github.com/taewoo1997/Portfolio/assets/108257288/0b364331-e4c4-4e32-9dcb-e78bfb49da6b)
프로젝트를 설치하고 실행하는 방법에 대한 안내를 작성합니다.

>
>

# 3. 공포 이야기 게시판



## 서비스 내용

공포 스토리를 글로 게시하거나, 실시간 채팅을 통해 접속자들끼리 다양한 이야기를 주고 받을 수 있습니다.

## 개발 기간

이 섹션에서는 프로젝트의 두 번째 기능에 대한 설명을 작성합니다.

## 개발 내용

이 섹션에서는 프로젝트의 세 번째 기능에 대한 설명을 작성합니다.

## 서비스 스크린샷
