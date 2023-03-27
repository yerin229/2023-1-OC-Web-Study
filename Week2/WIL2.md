# 기초 웹 스터디 2주차

복습: No
부제: GitHub
작성일시: 2023년 3월 26일 오전 2:30

### www.hongik.ac.kr을 입력하면 어떤 일이 일어날까?

Resource =  내가 얻고자 하는 대상

주소 = Resource가 저장된 주소

- URI (Uniform Resource Identifier)
    
    :Resource를 식별하는 통일된 방식
    
    ex) http://thinkzarahatke.com/author/amty.html#posts
    
- URL (Uniform Resource Location)
    
    : Resource를 얻을 수 있는 위치 (프로토콜+DNS주소)
    
    ex) [http://thinkzarahatke.com/author/amty.html](http://thinkzarahatke.com/author/amty.html-)
    
- URN (Uniform Resource Name)
    
    : Resource를 찾기 위한 이름
    
    ex) thinkzarahatke.com/author/amty.html#posts
    
    - 왜 이름을 사용할까?
        - 길고 복잡한 IP주고 외우고 관리하기 힘듦
        - IP주소는 사정에 따라 바뀔 수도 있음
    
    → DNS(Domain Name Server) 등장
    

허니콤보

ex) 교촌치킨 신촌점

ex) 허니콤보를 얻을 수 있는 위치를

알아내기 위한 방식

ex) 교촌치킨 신촌점

ex) 교촌치킨

### 웹페이지 구성

- HTML: 자료(뼈대) → 글만 있음
- CSS: UI(살과 옷) → 홈페이지 구성
- JavaScript: 제어 → 화면에서 움직이는 것들 멈춤

### GIT이란?

: 한 코드를 여러 사람이 같이 보고 수정 가능

- branch(분기): 하나의 코드가 나뭇가지가 갈라지둣 나누어짐
    - 분기 나누기, 분기 합치기, 변화 추적 가능, 특정 시점으로 되돌아가기 가능

### 파일의 4가지 상태


![Untitled](https://user-images.githubusercontent.com/127593340/227828606-3a3b5911-e9a0-409c-9f8b-8e136827e63c.png)
 Untracked (추적X)    Unmodified (변경X)        Modified(변경)                  Staged

       

![Untitled 1](https://user-images.githubusercontent.com/127593340/227828594-0fb8b56f-a13e-4034-8333-a418e1f788d2.png)

           Working Directory — add —> Staging Area — commit —> local repository

1. Working Directory (작업공간)
    
    : 내가 코드를 짜고 있는 공간
    
2. git add 명령어
    
    : Working Directory에서 git add 명령어 통해 Staging Area로 옮김 
    
3. Staging Area (준비 공간)
    
    : Working Directory에서 Staging Area로 변화들을 쌓아두는 공간
    
4. git commit 명령어
    
    : Staging Area에 쌓인 변화들을 논리적으로 엮어 git commit 명령어로 commit (수정된 내용을 데이터베이스에 저장)
    
5. Local Repository
    
    : commit을 마친 코드가 저장되는 저장소
    

ex) 사장님이 교촌 허니콤보 기능 구현해오라고 함

      치킨 만들기

              →

      소스 개발하기

1. 닭 손질
2. 염지
3. 튀김옷 입히기
4. 맛있게 튀기기
5. 소스 연구
6. 소스 테스트 해보기
7. 소스 선정
8. 소스 바르기

→ 사장님은 완성본(오른쪽) 보고 내가 뭘 했고 뭘 의도했는지 알 수 없음

**∴ staging area, local area** 구분

- 닭 손질, 염지, 튀김까지 Staging Area에 add → “치킨 만들기”라는 이름으로 Local Repository에 commit
- 소스 연구&테스트, 선정, 바르기까지 Staging Area에 add → “소스 개발하기”라는 이름으로 Local Repository에 commit

![Untitled 2](https://user-images.githubusercontent.com/127593340/227828602-3f59cd9e-b0c2-43c0-95ee-670eb27f6aae.png)
위의 과정은 모두 내 컴퓨터 안에서 일어난 일 **∴Remote Repository(외부 저장소)로 이동**

- Remote Repository
    
    : 내 컴퓨터 안에서 일어난 일을 저장하는 서버 → 여러 사람이 공유 가능
    

![Untitled 3](https://user-images.githubusercontent.com/127593340/227828604-82fc9ecc-bb39-46a9-a41a-dcab24d49220.png)

1. push 명령어
    
    : Local Repository에 저장된 변경 내용을 Remote Repository로 보내는 명령어
    
2. pull 명령어
    
    : Remote Repository의 변경사항 중 Local Repository에 반영되지 않은 내용을 가져올 때 사용
    
    기본 작동 - 현재 checkout 되어있는 branch의 내용 병합
    
3. fetch 명령어
    
    : Remote Repository의 변경사항을 가져오기만 하고, 현재 branch에 병합하지 않을 때 사용
    

+) 복잡한 병합의 경우 fetch를 사용하기 보다는 임시 branch를 새로 만들어 pull을 수행하고, rebase 명령을 통해서 작업 branch와 병합하는 방법을 사용합니다.
