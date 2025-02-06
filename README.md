# board
혼자서 A부터 Z까지 부딪히며 해보는 게시판 프로젝트

# 목표
하나하나 부딪혀가면서 개발하기. -> 깨달은 점에 대해 학습해나가기. 
목적, 문제점, 장점, 단점 등 생각해보기

# concept


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

# 나의 Branch 전략 ( 비록 1인 작업이지만... 협업 시에 대비해서 )
```
Git flow 방식 사용
feature : 작업 브랜치 / develop 브랜치를 기준으로 생성한다.
develop : Deploy-ready 상태의 코드가 있는 브랜치와 새로운 브랜치 생성의 base가 되는 브랜치, develop 브랜치에 들어왔다는 것은 테스트가 완료되었고 언제든 배포 가능하다는 뜻.
release : 배포 나갈 시 생성하는 브랜치 / develop 브랜치를 기준으로 생성 / 배포 & 모니터링 이후에는 master 브랜치로 머지한다.
master : Stable한 코드의 저장소, master 브랜치로 배포 시 언제든 stable 한 상태의 코드가 배포되게 한다.

각각의 이슈에 대한 개발 사항은 feature/이슈번호로 설정한다.

```
