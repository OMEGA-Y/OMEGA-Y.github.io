---
layout: post
title: "Git 정복하자 : Git remote 관련 기능"
---

#### `git remote -v` : 현재 폴더에 등록된 github 저장소를 확인할 때 사용한다.

#### `git remote add 저장소별명 저장소url` : 현재 폴더에 github 저장소를 연결할 때 사용한다. 저장소별명은 내가 임의로 지정하는 이름표라고 생각하면 된다. 아무 때나 변경할 수 있다. 보통 별명으로 origin이나 upstream을 많이 사용한다. 저장소url은 github 저장소 url이다. 

#### `git remote rename 현재저장소별명 변경하려는이름` : 현재 폴더에 연결된 github저장소 별명을 변경할 때 사용한다. 

#### `git remote rm 삭제하려는저장소별명` : 현재 폴더에 등록된 github 저장소를 삭제할 때 사용한다.

#### `git clone 복제하려는저장소url` : 원하는 Git 저장소를 로컬 서버로 복사하고 싶을 때 사용한다. 보통 프로젝트에 참여할 때 fork를 뜬 후 내 repository에서 HTTPS url을 복사해서 clone 뒤에 입력하면 된다.

