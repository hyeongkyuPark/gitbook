---
description: HTML에서 JavaScript 조건문을 활용하여 2가지의 버튼을 한 개로 통합
---

# HTML 조건문 활용

* html의 속성값을 이용해서 특정 속성값이 할당되어 있는경우에만 실행되는 코드를 작성하여 분기가능
* 배경 색상을 검정색 또는 하얀색으로 변경할 때 if문을 사용하여 버튼 한개에 이미 검정색일 때는 흰색으로 변경하고 그렇지 않을경우 검정색으로 변경해주는 조건문을 작성하면 통합할 수 있음

```markup
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title></title>
</head>
<body>
  <input type="button" value="toggle" onclick="
    var bodyTag = document.querySelector('body');
    if(bodyTag.style.backgroundColor === 'black') {
      bodyTag.style.backgroundColor = 'white';
      bodyTag.style.color = 'black';                                         
    } else {
        bodyTag.style.backgroundColor = 'black';
        bodyTag.style.color = 'white';
    }
  "/>
  <h1>HTML&조건문</h1>
  <p>
    자바스크립트(JavaScript)는 객체(object) 기반의 스크립트 언어입니다.
HTML로는 웹의 내용을 작성하고, CSS로는 웹을 디자인하며, 자바스크립트로는 웹의 동작을 구현할 수 있습니다.
자바스크립트는 주로 웹 브라우저에서 사용되나, Node.js와 같은 프레임워크를 사용하면 서버 측 프로그래밍에서도 사용할 수 있습니다.
현재 컴퓨터나 스마트폰 등에 포함된 대부분의 웹 브라우저에는 자바스크립트 인터프리터가 내장되어 있습니다.
  </p>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/qBrYoXL" %}



