#### What I learned?
- Git Log : commit의 기록을 최신순으로 확인한다. --online을 사용하면 각 커밋을 요약해서 보여준다.

- Commit ID : 각 커밋을 식별하기 위해 사용되는 40자리의 16진수 수.  
중복될 확률은 2의 80제곱 분의 1이며, SHA-1 해시 함수를 사용한다.

- HEAD : 현재 작업 중인 commit의 위치. 가장 최근 커밋에 해당되며, 다음 commit의 base이기도 하며, 새로운 commit이 생기면 HEAD도 바뀐다.

- git status : 세 가지 상태에 따라 파일을 분류하여 확인한다.

- commit --amend : 마지막 commit에 변경이 있을 때 사용된다.  
새로운 commit으로 대체되는 것이기에 commid id도 바뀌며, vim으로 진입해 commit message를 수정하게 된다.  
-m 옵션을 사용해 vim으로 진입하지 않고 commit message를 수정하거나, --no-edit 옵션을 사용해 메시지의 수정 없이 commit을 수정할 수 있다.  
다른 사람의 commit에 --amend 옵션을 사용하면 안된다.

- reset : commit id를 사용하여 commit을 제거하는 데에 사용된다.
- reset --soft : commit만 취소되며, 변경 사항이 staging area로 돌아간다.
- reset --mixed : commit이 취소되며, 변경 사항이 working directory로 돌아간다.
- reset --hard : commit이 취소되며, 변경 사항을 모두 제거하고 이전 commit으로 돌아간다.

- revert : commit을 되돌리는 기능. 현재 commit을 보존한 채 이전 commit을 새로운 commit으로써 불러온다.
- revert --no-edit : 편집기 진입 없이 바로 commit한다.
- revert --no-commit : 직접 commit하지 않고, revert 내용을 바로 staging area에 올린다.  

- reset은 commit을 삭제하기 때문에 위험하고, 다른 브랜치에도 영향을 줄 수 있으므로, revert가 안전하다.