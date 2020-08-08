---
layout: post
title: "Git 정복하자 : Git remote 관련 기능"
---

###### ==git remote -v== : 현재 폴더에 등록된 github 저장소를 확인할 때 사용한다.

###### ==git remote add== <span style="color:blue">저장소 별명</span>  <span style="color:red">저장소 url</span> : 현재 폴더에 github 저장소를 연결할 때 사용한다. 파란 부분은 내가 임의로 지정하는 이름표라고 생각하면 된다. 아무 때나 변경할 수 있다. 보통 별명으로 origin이나 upstream을 많이 사용한다. 빨간 부분은 github 저장소 url이다. 

###### ==git remote rename == <span style="color:blue">현재 저장소 별명</span>  <span style="color:red">변경하려는 저장소 별명</span> : 현재 폴더에 연결된 github저장소 별명을 변경할 때 사용한다. 

###### ==git remote rm == <span style="color:blue">삭제하려는 저장소 별명</span> : 현재 폴더에 등록된 github 저장소를 삭제할 때 사용한다.

###### ==git clone== <span style="color:blue">복제하려는 저장소 url</span> : 원하는 Git 저장소를 로컬 서버로 복사하고 싶을 때 사용한다. 보통 프로젝트에 참여할 때 fork를 뜬 후 내 repository에서 HTTPS url을 복사해서 clone 뒤에 입력하면 된다.