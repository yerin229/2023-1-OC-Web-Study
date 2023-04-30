# 기초 웹 스터디 5주차

복습: No
부제: css
작성일시: 2023년 4월 11일 오후 6:17

## HTML

1. 요소
    
    :검색시 해석하는 대상
    
    - non-semantic 요소
        
        : 태그는 content에 대해 어떤 설명도 하지 않음
        
        ex) div, span 등
        
    - semantic 요소
        
        : 태그는 content의 의미를 명확히 설명
        
        ex) form, table, img 등
        
2. 태그
    - 문서 형식 정의 tag
        
        출력할 웹페이지의 형식 브라우저에 전달
        
    - HTML tag
        
        모든 HTML 요소의 부모 요소 (단 하나만 존재)
        
    - head tag
        
        meta data 포함 위한 요소 (단 하나만 존재)
        
        화면에 표시 X
        
    - title tag
        
        문서의 제목 정의 (브라우저의 탭에 표시)
        
    - style tag
        
        HTML 문서 위한 style 정보 정의
        
    - link tag
        
        외부 리소스와의 연계 정보 정의 (주로 HTML과 외부 CSS 파일)
        
    - script tag
        
        client-side JavaScript 정의
        
    - meta tag
        
        description, keywords, author, 기타 메타데이터 정의
        
        브라우저, 검색 엔진 등에 의해 사용
        
    - body tag
        
        HTML 문서의 내용 (단 하나만 존재)
        
        meta data 제외한 대부분의 요소가 기술되는 곳
        

## CSS: Cascading Style Sheet

(스타일을 정해주는 기능)

### Cascading: 위에서부터 내려오는 상속(종속) 관계

- 특징1: 상속관계
    - 부모의 스타일을 자식에게 상속 가능
- 특징2: 우선순위
    - 한 요소에 여러 스타일이 적용된다면 무엇을 우선 순위로 두어야 하는지
    - 우선순위:
        
        ![2.jpg](https://user-images.githubusercontent.com/127593340/235364849-a9566729-a233-4cf3-959c-0387673856da.jpg)
        
        1. 사용자 스타일(컴퓨터 사용자) 
            
            ex) 다크모드 설정 등
            
        2. 제작자 스타일(개발자)
            1. !important
            2. 인라인 스타일
            3. id 스타일
            4. 클래스 스타일
            5. 타입 스타일
            
            ![Selector 통해 적용 가능](https://user-images.githubusercontent.com/127593340/235364750-b541d3d7-7634-4f8b-adcd-6a51a7ade0d7.png)
            
            Selector 통해 적용 가능
            
            [Selector 종류]
            
            - id 선택자: #아이디 {속성 : 값 … }
                - 특정 아이디 가진 요소에 적용
            - 클래스 선택자: .클래스 {속성 : 값 … }
                - 특정 클래스 가진 모든 요소에 적용
            - 타입 선택자: 태그 {속성 : 값 … }
                - 특정 태그 사용한 모든 요소에 적용
            - 전체 선택자 * {속성 : 값 … }
                - 문서의 모든 요소에 적용
        3. 브라우저 기본 스타일

## HTML과 CSS 의 연동

- Link Style (가장 일반적)
    
    : HTML 외부에 있는 CSS 파일 로드
    
- Embedding Style
    
    : HTML 내부에 CSS 포함시키는 방식
    
    매우 간단한 웹페이지의 경우는 문제 X  but HTML과 CSS는 역할 다르므로 다른 파일로 구분해 작성&관리가 바람직
    
- Inline Style
    
    : HTML 요소의 style 프로퍼티에 CSS 기술
    
    Java Script가 동적으로 CSS  생성할 때 사용하는 경우 존재
    
- Reset CSS  사용
    
    기본적인 HTML 요소의 CSS 초기화하는 용도 (브라우저 별로 제각각인 디폴트 스타일 하나로 통일)
