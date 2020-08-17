---
layout: post
title: [확장자 js 파일] document is not defined"
---

#### js 파일에서 document.write() 사용할 때 주의사항
![에러난 이미지](https://github.com/OMEGA-Y/OMEGA-Y.github.io/blob/master/_img/document.write()%20%EA%B4%80%EB%A0%A8%20%EC%97%90%EB%9F%AC.jpg)

위 이미지에서 `document is not defined`를 보면 된다. 일단 이 파일의 확장자는 `.js`이고 `document.write()`을 이용해 output에 계산 결과를 출력하려고 한다. ReferenceError가 났는데 검색해보니까 node.js는 DOM 객체가 내장되어 있지 않아 나는 에러다. DOM(Document Object Model)은 브라우저에는 내장되어 있지만 JS에는 내장되어 있지 않으므로 따로 `npm install jsdom`' 코드로 설치해줘야 한다.<br> 이렇게 설치하고 추가로 무언가 더 해야하는 것 같은데 지금 내 상태로는 이해 못하겠어서.... 주변에 도움을 청하였고... 쉽게 해결될 거 같지 않아 그냥 출력 함수를 다른걸로 사용하기로 했다... <br>일단 html에 script태그로 삽입하거나 console.log를 사용해야겠다.




