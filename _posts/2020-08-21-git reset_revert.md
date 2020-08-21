---
layout: post
title: "Git 정복하자 : Git reset/revert"
---

### reset : commit 지울 때
##### hard와 soft로 나뉜다. hard 타입으로 reset할 경우 commit할 때 올렸던 수정사항과 commit 기록 모두 지워진다. soft 타입으로 reset할 경우 commit할 때 올렸던 수정사항은 남아있고, commit 기록만 지워진다.

#### 사용법
`git reset --hard HEAD~1` 또는 `git reset --soft HEAD~1`: 1 자리에는 삭제하고 싶은 commit의 개수를 입력하면 된다. 현재 HEAD로 부터 몇 개의 commit을 삭제할지 의미하는 것이다.

<br>
### revert : 잘못 올라간 commit을 되돌리고 싶을 때
##### 다른 사람들과 공유하는 원격 저장소에 올라간 commit 중 되돌리고 다시 commit하고 싶은 상황에서 revert를 하게 된다. revert를 하게 되면 revert에 대한 commit이 생성되고, revert한 commit에 들어있던 파일 변경사항이 초기화된다.

#### 사용법
`git revert commitID` : log에 있는 commitID를 복붙하면 된다.

<br>  
_JS study repo에서 실수하며 확실하게 알게 됨_
### revert와 reset의 차이점
가장 큰 차이는 **다른 사람과 공유하는 repository에서 reset은 하면 안 되고 revert는 해도 된다는 것**이다. 예를 들어, 내가 올린 commit이 공동 repo에 merge 되고 다른 사람의 commit이 그 위로 여러 개 merge 되었다고 하자. 이 때, 이미 merge된 commit들을 내 로컬 repo에서 reset 하더라도 이 상태를 원격 repo로 반영하지는 못한다. 따라서 내 commit에 대한 결과물을 다시 되돌리고 원하는 방향으로 수정해 공동 repo에 반영하려면 다음과 같이 해야 한다. <br>
<br>1. git log --oneline으로 해당 commit 아이디를 알아낸 후 revert 한다.
<br> 2. 수정한 파일을 add하고 새롭게 commit한다.
<br> 3. revert 하면서 생긴 commit과 새롭게 만든 commit 2개를 내 repo에 push하고 공동 repo에 PR을 보낸다.
<br> 4. 공동 repo에서 merge 되면 결과가 반영된다!


