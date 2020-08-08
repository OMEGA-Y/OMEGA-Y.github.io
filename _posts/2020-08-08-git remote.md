---
layout: post
title: "Git 정복하자 : Git remote 관련 기능"
---

#### remote 저장소 연결
**`git remote -v`** : 현재 폴더에 등록된 github 저장소를 확인할 때 사용한다.
<br>
**`git remote add 저장소별명 저장소url`** : 현재 폴더에 github 저장소를 연결할 때 사용한다. 저장소별명은 내가 임의로 지정하는 이름표라고 생각하면 된다. 아무 때나 변경할 수 있다. 보통 별명으로 origin이나 upstream을 많이 사용한다. 저장소url은 github 저장소 url이다. 
<br>
**`git clone 복제하려는저장소url`** : 원하는 Git 저장소를 로컬 서버로 복사하고 싶을 때 사용한다. 보통 프로젝트에 참여할 때 fork를 뜬 후 내 repository에서 HTTPS url을 복사해서 clone 뒤에 입력하면 된다.
<br>
<br>
#### remote 저장소 이름변경 및 삭제
**`git remote rename 현재저장소별명 변경하려는이름`** : 현재 폴더에 연결된 github저장소 별명을 변경할 때 사용한다. 
<br>
**`git remote rm 삭제하려는저장소별명`** : 현재 폴더에 등록된 github 저장소를 삭제할 때 사용한다.
<br>
<br>
#### remote 브랜치 생성 및 삭제
**`git push origin(저장소별명) 브랜치이름`** : 로컬에서 브랜치를 새로 생성한 후 브랜치 작업 결과를 commit 하여 원격저장소에 push하고 싶을 때 사용한다. 원격저장소에 branch를 새롭게 생성함과 동시에 현재의 로컬 브랜치와 생성된 원격 서버의 브랜치를 동기화시킨다. 저장소별명을 적는 부분에 대부분의 경우 origin을 적으면 될 것 같다.
<br>
**`git push origin(저장소별명) :브랜치이름`** 또는 **`git push origin --delete 브랜치이름`**: 원격 저장소의 브랜치를 삭제하고 싶을 때 사용한다. 브랜치이름에 삭제하려는 브랜치 이름을 넣으면 된다.
<br>

