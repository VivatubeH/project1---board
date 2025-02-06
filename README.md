# board
혼자서 A부터 Z까지 부딪히며 해보는 게시판 프로젝트

# 목표
하나하나 부딪혀가면서 개발하기. -> 깨달은 점에 대해 학습해나가기. 
목적, 문제점, 장점, 단점 등 생각해보기

# 스스로의 다짐
시작부터 모든 걸 설계하기는 어려우니, 모든 걸 시작부터 의존성 주입한다기보다는 프로젝트를 해나가면서 수정하기,
디자인에 너무 신경쓰지 않게 부트스트랩 라이브러리를 활용하고, 실질적인 구현 및 설계에 집중하기.

# 활용해 볼만한 툴
AWS(온라인상에서 실행을 위한 서버 대여), 젠킨스 ( 빌드 배포 자동화 도구 ), docker ( 컨테이너 만들기 ) 등 때에 따라 필요한 기술들 아키텍처나 간단한 사용법 익히고 실전에 적용하면서 배우기

# concept
일반적인 커뮤니티 게시판, 익명 게시판, 특정한 폼이 있는 게시판( 예: QnA ), 공지사항 게시판, 신고 게시판 등 각각의 목적에 맞는 게시판 설계 및 구현하기.

# Project Convention
1. UI : Bootstrap
2. Template : JSP

# Environment
1. java :
2. oracleSQL :
3. Default Encoding :
4. Default File System :

# IDE

# Build

# Reference Documentation
[깃 브랜치 전략]
- https://inpa.tistory.com/entry/GIT-%E2%9A%A1%EF%B8%8F-github-flow-git-flow-%F0%9F%93%88-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EC%A0%84%EB%9E%B5

# 나의 Branch 전략 
```
Git flow 방식 사용
feature : 작업 브랜치 / develop 브랜치를 기준으로 생성한다.
develop : Deploy-ready 상태의 코드가 있는 브랜치와 새로운 브랜치 생성의 base가 되는 브랜치, develop 브랜치에 들어왔다는 것은 테스트가 완료되었고 언제든 배포 가능하다는 뜻.
release : 배포 나갈 시 생성하는 브랜치 / develop 브랜치를 기준으로 생성 / 배포 & 모니터링 이후에는 master 브랜치로 머지한다.
master : Stable한 코드의 저장소, master 브랜치로 배포 시 언제든 stable 한 상태의 코드가 배포되게 한다.

각각의 이슈에 대한 개발 사항은 feature/이슈번호로 설정한다.
feature/이슈번호에서 개발한 각각의 기능은 게시판의 종류에 따라 feature/게시판종류/날짜 브랜치로 통합한다.

feature/게시판종류/날짜 브랜치에서 develop 브랜치로 통합한다.

develop 브랜치에서 테스트를 해보고 괜찮으면 release -> master 순서로 배포한다.

배포 과정을 익히는 동안은 feature -> feature/도메인 -> develop으로 가는 일련의 과정만 수행한다.
```
