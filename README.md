# 포트폴리오 프로젝트 소개
개인 프로젝트를 소개합니다.
- [**vision 북체커**](#vision-북체커)
- [**딥러닝 모델 기반 실시간 전신주 균열 탐지 및 통합관리 애플리케이션**](#딥러닝-모델-기반-실시간-전신주-균열-탐지-통합관리-애플리케이션)
  
# vision 북체커

도서관 서가 배열 순서 확인 애플리케이션

## 목차

- [프로젝트 개요](#프로젝트-개요)
- [개발 기간](#개발-기간)
- [섹션 3: 기능 3](#섹션-3-기능-3)
- [섹션 4: 스크린샷](#섹션-4-스크린샷)
- [섹션 5: 데모](#섹션-5-데모)
- [섹션 6: 설치 및 실행](#섹션-6-설치-및-실행)

## 프로젝트 개요

이 섹션에서는 프로젝트의 첫 번째 기능에 대한 설명을 작성합니다.

## 개발 기간

이 섹션에서는 프로젝트의 두 번째 기능에 대한 설명을 작성합니다.

## 섹션 3: 기능 3

이 섹션에서는 프로젝트의 세 번째 기능에 대한 설명을 작성합니다.

## 섹션 4: 스크린샷

![청구기호1](https://github.com/taewoo1997/Portfolio/assets/108257288/1691dab8-1ac1-44bb-b1f6-0474a2d338c0)

![청구기호1_OCR](https://github.com/taewoo1997/Portfolio/assets/108257288/be91c440-bf67-4224-941f-dd1114564467)

스크린샷에 대한 간단한 설명을 작성합니다.

## 섹션 5: 데모

![객체탐지](https://github.com/taewoo1997/Portfolio/assets/108257288/b90f4e01-395a-4190-b52c-453c6fa59cb7)

프로젝트의 데모를 보여주는 GIF 파일과 간단한 설명을 작성합니다.

## 섹션 6: 설치 및 실행

프로젝트를 설치하고 실행하는 방법에 대한 안내를 작성합니다.

>
> 

# 딥러닝 모델 기반 실시간 전신주 균열 탐지 <br>통합관리 애플리케이션

딥러닝 기반 드론을 활용한 전신주 균열 탐지 시스템

## 목차

- [프로젝트 개요](#프로젝트-개요)
- [개발 기간](#개발-기간)
- [섹션 3: 기능 3](#섹션-3-기능-3)
- [섹션 4: 스크린샷](#섹션-4-스크린샷)
- [섹션 5: 데모](#섹션-5-데모)
- [섹션 6: 설치 및 실행](#섹션-6-설치-및-실행)

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

## 섹션 5: 데모



프로젝트의 데모를 보여주는 GIF 파일과 간단한 설명을 작성합니다.

## 섹션 6: 설치 및 실행

프로젝트를 설치하고 실행하는 방법에 대한 안내를 작성합니다.
