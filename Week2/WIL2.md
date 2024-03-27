#### What I Learned Today?
- Fork : 다른 사용자의 레포지토리를 자신의 계정으로 복사하여 독립적으로 수정하고 관리하는 것.  
- Star : 북마크 기능처럼, 관심있는 레포지토리나 프로젝트에 star를 달아 관리하는 것.  
- Issue : 레포지토리에서 작업 계획, 토론 및 추적을 위해 활용하는 것.  
- Branch : 기본 브랜치에서 분리되어 생성되는 별도의 작업 공간. fork와는 다르게 같은 레포지토리에서 생성된다.  
- 브랜치 네이밍 팁 : (이슈의 유형/이슈의 번호-간략한 설명)  
- Pull Request : 분기된 브랜치를 기존 브랜치와 병합하는 절차. 새로운 변경을 제안하거나, 병합시에 발생하는 충돌을 해결한다. 또, Merge에 앞서 코드를 리뷰한다.  
- Merge에는 3가지 옵션이 존재한다.
1. Merge Commit : 두가지 브랜치를 공통 부모로 삼는 새로운 commit을 만들고, 분기된 commit이 그대로 main 브랜치에 통합된다.
2. Sqaush and Merge : 분기된 commit을 squash 해서 하나의 commit으로 만들어 main 브랜치에 통합한다.
3. Rebase and Merge : 분기된 commit의 base를 재설정하여 새로운 commit으로 변경하고, commit hash도 변경된다. 충돌에 주의.
- commit hash 란? commit의 식별을 위해 사용되는 40자 길이의 16진수

#### What I Do?
1. Issue 생성하기
2. 현재 브랜치를 확인하기(git branch)
3. 브랜치 생성하기(git branch "이름"), 브랜치 삭제하기(git branch -D "이름")
4. 브랜치 이동하기(git checkout "이름")
-브랜치 생성하고 이동하기(git checkout -b "이름")
5. Pull Request 만들기
6. Squash and Merge 통해 README.md 교체하기

- [GDSC 개발 입문 스터디 2주차 과제](https://github.com/daenykevin/2024-1-Beginner-Study/pull/2)