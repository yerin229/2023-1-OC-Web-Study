# 기초 웹 스터디 6주차

복습: No
부제: css, html
작성일시: 2023년 5월 7일 오후 10:22

## <Box Model>

앞 시간에 배운 요소들=보이지 않는 박스 안에 있었다 (테두리X)

![Content → Padding → Border → Margin](%E1%84%80%E1%85%B5%E1%84%8E%E1%85%A9%20%E1%84%8B%E1%85%B0%E1%86%B8%20%E1%84%89%E1%85%B3%E1%84%90%E1%85%A5%E1%84%83%E1%85%B5%206%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%200b15ca2d802049e586fa082d563132a0/Untitled.png)

Content → Padding → Border → Margin

*border: 테두리

*Padding: Content와 Border 사이의 간격

*Margin: Border과 다른 Content 사이의 여백

1. 블록 레벨 요소
    
    : 한 줄을 차지하는 박스
    
    - 부모 요소의 전체 칸 차지

1. 인라인 레벨 요소
    
    : 자신만을 감싸는 박스
    
    - 부모 요소 안에서 나뉠 수 있음

![Untitled](%E1%84%80%E1%85%B5%E1%84%8E%E1%85%A9%20%E1%84%8B%E1%85%B0%E1%86%B8%20%E1%84%89%E1%85%B3%E1%84%90%E1%85%A5%E1%84%83%E1%85%B5%206%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%200b15ca2d802049e586fa082d563132a0/Untitled%201.png)

## <FLEX Box Layout & Grid Box Layout(Grid 생략)>

- FLEX Box Layout → Flexible layout
- 아이템이 배열될 방향(주축)정할 수 있음]
    
    main axis: 주축
    
    cross axis: 주축과 수직인 축
    
- justify-content: main axis
    - flex-start (default) ⇒ 요소들을 컨테이너의 왼쪽으로 정렬
    - flex-end ⇒ 요소들을 컨테이너의 우측으로 정렬
    - center ⇒ 요소들을 컨테이너의 중앙으로 정렬
    - space-between ⇒ 요소들 사이에 동일한 간격
    - space-around ⇒ 요소들 주위에 동일한 간격을 둡니다.
- align-item: cross axis
    - flex-start ⇒ 컨테이너의 최상단으로 정렬
    - flex-end ⇒ 컨테이너의 최하단으로 정렬
    - center ⇒ 컨테이너의 세로 축의 중앙으로 정렬
    - baseline ⇒ 컨테이너의 시작위치에 정렬
    - stretch(default) ⇒ 컨테이너에 맞게 늘림
    

## <Flexbox Froggy 답>

1.  justify-content: flex-end
2. justify-content: center
3. justify-content: space-around;
4. justify-content: space-between;
5. align-items: flex-end;
6. justify-content: center;
align-items: center;
7. justify-content: space-around;
align-items: flex-end;
8. flex-direction: row-reverse;
9. flex-direction: column;
10. flex-direction: row-reverse;
justify-content: flex-end;
11. flex-direction: column;
justify-content: flex-end;
12. flex-direction: column-reverse;
justify-content: space-between;
13. flex-direction: row-reverse;
justify-content: center;
align-items: flex-end;

18. flex-wrap: wrap;

1. flex-direction: column;
flex-wrap: wrap;
2. flex-flow: column wrap;