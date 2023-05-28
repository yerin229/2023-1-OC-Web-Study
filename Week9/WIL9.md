# 기초 웹 스터디 9주차

복습: No
부제: js
작성일시: 2023년 5월 28일 오후 10:34

## 브라우저 동작 원리

- 브라우저는 동기적으로 HTML, CSS, Javascript을 처리
- 브라우저는 서버로부터 HTML, CSS, Javascript, 이미지 파일 등을 응답
    
    → HTML, CSS 파일은 렌더링 엔진의 HTML 파서와 CSS 파서에 의해 파싱 → HTML, CSS 파일은 렌더링 엔진의 HTML 파서와 CSS 파서에 의해 파싱
    
    ![1](https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/eaa6a31d-eb62-4c92-939b-886e5432554e)
    

## 객체

- key와 value로 구성된 property들의 집합 (property value가 함수일 경우 → 메소드)
- 자바 스크립트를 이루고 있는 거의 모든 것 (원시 타입을 제외한 나머지 값들)
- 객체 생성 방법
    - 객체 리터럴: 중괄호를 사용해 객체 생성
    - object 생성자 함수
    - 생성자 함수
- 객체의 분류
    
    ![2](https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/49ced528-2a8e-4b56-992c-34f32a5a9cc5)
    

## 함수

- 어떤 작업을 수행하기 위해 필요한 statement들의 집합을 정의한 코드 블록
- 함수 정의 방식
    - 함수 선언문
        - function 키워드, 함수명, 매개변수 목록, 함수 몸체
    - 함수 표현식
        - 함수의 일급 객체 특성을 이용해 함수 리터럴 방식으로 함수 정의&변수에 할당
    - Function 생성자 함수
        - 위의 방법은 Function 생성자 함수로 함수 생성하는 것을 단순화 시킨 축약법

## 배열

- 1개의 변수에 여러개의 값 순차적 저장할 때 이용
- 배열 생성
    - 배열 리터럴
        - 0개 이상의 값을 쉼표로 구분해 대괄호로 묶음
    - Array() 생성자 함수
        - 위의 방법은 Array() 생성자 함수로 배열을 생성하는 것을 단순화

## 문서 객체 모델 DOM

- 모든 요소와 요소의 어트리뷰트, 텍스트를 각각의 객체로 만들고 이들 객체를 부자 관계를 표현할 수 있는 트리 구조로 구성한 것
- 기능
    - HTML 문서에 대한 모델 구성
    - HTML 문서 내의 각 요소에 접근/수정

## 이벤트

- 이벤트 종류
    - UI Event
        
        <img width="430" alt="3" src="https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/b7ab9bdc-d4c5-41b5-849f-af2735e51a7f">
        
    - Keyboard Event
        
        <img width="430" alt="4" src="https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/5a9ca8a2-8f8c-4e9d-83a0-d335382ed8e4">
        
    - Mouse Event
        
        <img width="429" alt="5" src="https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/c7fdfb48-1309-4124-b3d2-bdebbc576e82">
        
    - Focus Event
        
        <img width="427" alt="6" src="https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/574ba6a6-1b87-44a6-b3c2-c4338314e83c">
        
    - Form Event
        
        <img width="431" alt="7" src="https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/b5e9bd18-e417-461b-9b2d-62cc83aac129">
        
    - Clipboard Event
        
        <img width="430" alt="8" src="https://github.com/yerin229/2023-1-OC-Web-Study/assets/127593340/aa557c97-d657-4c41-9bf3-ae99f8d8a26a">
        
- 이벤트 핸들러 등록
    - 인라인 이벤트 핸들러 방식
        - HTML 요소의 이벤트 핸들러 어트리뷰트에 이벤트 핸들러 등록
    - 이벤트 핸들러 프로퍼티 방식
        - HTML과 Javascript 섞이는 문제 해결
        - 이벤트 핸들러 프로퍼티에 하나의 이벤트 핸들러만 바인딩 가능
    - addEventListener 메소드 방식
        - addEventListener 메소드를 사용해 대상 DOM 요소에 이벤트 바인딩&해당 이벤트 발생 시 실행될 콜백 함수(이벤트 핸들러) 지정
