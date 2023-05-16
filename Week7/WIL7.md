# 기초 웹 스터디 7주차

복습: No
부제: css, html, js
작성일시: 2023년 5월 14일 오후 8:46

## <사이트 분석&구현>

1. 구획 나누기
    
    ![구획 나누기.png](%E1%84%80%E1%85%B5%E1%84%8E%E1%85%A9%20%E1%84%8B%E1%85%B0%E1%86%B8%20%E1%84%89%E1%85%B3%E1%84%90%E1%85%A5%E1%84%83%E1%85%B5%207%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%208349e4adab4b46d1bd99f087a45a78c5/%25EA%25B5%25AC%25ED%259A%258D_%25EB%2582%2598%25EB%2588%2584%25EA%25B8%25B0.png)
    
    ![구획 이름.png](%E1%84%80%E1%85%B5%E1%84%8E%E1%85%A9%20%E1%84%8B%E1%85%B0%E1%86%B8%20%E1%84%89%E1%85%B3%E1%84%90%E1%85%A5%E1%84%83%E1%85%B5%207%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%208349e4adab4b46d1bd99f087a45a78c5/%25EA%25B5%25AC%25ED%259A%258D_%25EC%259D%25B4%25EB%25A6%2584.png)
    
2. flex 이용한 배치
    - view 안에 header와 container ⇒ flex-direction : columns
    - header 안에 각종 버튼들 ⇒ row
    - container 안에 main-container와 aside-container ⇒ row
    - main-container 안에 3개의 container ⇒ columns
    - video-info-container 안에 제목, 게시자 정보 ⇒ columns
    - comment-container 안에 댓글 ⇒ columns
3. CSS 초기화&기본 index.html 틀 작성
    
    브라우저 스타일을 초기화 ⇒ 모든 브라우저에 동일한 스타일을 적용 (필수X)
    
4. Header
    1. Search Bar
5. 컨테이너
    1. main container
    2. video-container
    3. video-info-container
        1. 채널 정보의 버튼들
        2. discription
        3. drop-down
    4. comment-container
    5. aside-container