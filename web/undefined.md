---
description: javascript를 이용해 DOM(html 요소)를 선택하는 방법
---

# 선택하기

## 📕 아이디로 선택하기

* Html 태그의 속성인 id를 이용해 ElementDOM을 선택하는 방법으로는 document.getElementById\(\) 메서드가 있음
* id는 태그에 고유값을 부여해주는 속성으로 같은 id값을 사용하는 것은 지양\(에러가 발생하지 않음\)
* ElementDOM은 style이라는 속성으로 css스타일에 값을 출력하거나 변경할 수 있음

```markup
<body id="body-tag">
    <!-- 버튼에 onclick 이벤트 속성으로 클릭시 발생할 이벤트 지 -->
    <input type="button" value="어둡게" onclick="
        // bodyTag변수에 id값으로 Element 할당
        var bodyTag = document.getElementById('body-tag');
        bodyTag.style.backgroundColor = 'black'; // 배경색 변경
        bodyTag.style.color = 'white' // 글자색 변
    " />
    <input type="button" value="밝게" onclick="
        var bodyTag = document.getElementById('body-tag');
        bodyTag.style.backgroundColor = 'white';
        bodyTag.style.color = 'black'
    " />
    <h1>HTML ID로 선택하기</h1>
    <p>
        자바스크립트는 ‘웹페이지에 생동감을 불어넣기 위해’ 만들어진 프로그래밍 언어입니다.
        자바스크립트로 작성한 프로그램을 스크립트(script) 라고 부릅니다. 스크립트는 웹페이지의 HTML 안에 작성할 수 있는데, 
        웹페이지를 불러올 때 스크립트가 자동으로 실행됩니다.
        스크립트는 특별한 준비나 컴파일 없이 보통의 문자 형태로 작성할 수 있고, 실행도 할 수 있습니다.
        이런 관점에서 보면 자바스크립트는 자바(Java)와는 매우 다른 언어라고 할 수 있습니다.
    </p>
</body>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/LYWmQQe" %}



## 📕 클래스로 선택하기

* Html의 속성중 하나인 class속성값을 이용해 선택하는 방법으로는 document.getElementsByClassName\(\)라는 메서드가 있음
* class 속성은 여러 html element에 적용할 수 있는 속성으로 유사 배열\(배열은 아니지만 배열과 같이 length 등 기능 제공\)의 형태를 반환함
* 하나의 태그에 여러가지 class를 지정할수도 있

```markup
<body id="body-tag">
    <!-- 버튼에 onclick 이벤트 속성으로 클릭시 발생할 이벤트 지 -->
    <input type="button" value="red" onclick="
        // languageItems변수에 class값으로 Element 유사배 할당
        var languageItems = document.getElementsByClassName('language-item');
        languageItems[0].style.color = 'red'; // 첫번째 요소 컬러 변
        languageItems[1].style.color = 'red'; // 두번째 요소 컬러 변
        languageItems[2].style.color = 'red'; // 번째 요소 컬러 변경
    " />
    <input type="button" value="blue" onclick="
        // languageItems변수에 class값으로 Element 유사배 할당
        var languageItems = document.getElementsByClassName('language-item');
        languageItems[0].style.color = 'blue'; // 첫번째 요소 컬러 변
        languageItems[1].style.color = 'blue'; // 두번째 요소 컬러 변경
        languageItems[2].style.color = 'blue'; // 번째 요소 컬러 변경
    " />
    <h1>HTML class로 선택하기</h1>
    <ul>
        <li class='language-item html'>html : 마크업 언어</li>
        <li class='language-item css'>css : html 스타일 언어</li>
        <li class='language-item js'>javascript : 동적 언</li>
    </ul>
</body>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/XWMqZYM" %}



## 📕 태그명으로 선택하기

* html tag의 이름을 이용해서 선택하는 방법은 document.getElementsByTagName\(\) 메서드를 사용
* 한 html 문서내에는 같은 tag들이 여러개 있을 수 있으므로 class를 선택하는 것과 마찬가지로 여러 element 들을 유사배열 형태로 반환

```markup
<body id="body-tag">
    <!-- 버튼에 onclick 이벤트 속성으로 클릭시 발생할 이벤트 지 -->
    <input type="button" value="selector" onclick="
        // languageItem변수에 class값으로 첫번 Element 할당
        var languageItem = document.querySelector('.language-item');
        languageItem.style.color = 'red'; // 첫번째 요소 컬러 변경
    " />
    <input type="button" value="selectorAll" onclick="
        // languageItems변수에 class값으로 Element 유사배 할당
        var languageItems = document.querySelectorAll('.language-item');
        languageItems[0].style.color = 'blue'; // 첫번째 요소 컬러 변
        languageItems[1].style.color = 'blue'; // 두번째 요소 컬러 변경
        languageItems[2].style.color = 'blue'; // 번째 요소 컬러 변경
    " />
    <h1>HTML class로 선택하기</h1>
    <ul>
        <li class='language-item html'>html : 마크업 언어</li>
        <li class='language-item css'>css : html 스타일 언어</li>
        <li class='language-item js'>javascript : 동적 언</li>
    </ul>
</body>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/poeVaOy" %}



## 📕 CSS 선택자로 선택하기

* css 선택자를 이용해 선택하는 방법은 document.querySelector\(\)와 document.querySelectorAll\(\)이 있음
* document.querySelector\(\) 메서드는 class나 tag와 같이 여러개의 결과값이 존재하더라도 가장 먼저 나오는 한 개의 결과만을 반환
* document.querySelectorAll\(\) 메서드는 해당하는 element가 여러개라면 유사배열의 형태로 모두 반환함

```markup
<body id="body-tag">
    <!-- 버튼에 onclick 이벤트 속성으로 클릭시 발생할 이벤트 지 -->
    <input type="button" value="red" onclick="
        // liItem변수에 Tag명을 탐색하여 Element 유사배열 할당
        var liItem = document.querySelector('li');
        liItems[0].style.color = 'red'; // 첫번째 요소 컬러 변경
        liItems[1].style.color = 'red'; // 두번째 요소 컬러 변
        liItems[2].style.color = 'red'; // 번째 요소 컬러 변경
    " />
    <input type="button" value="blue" onclick="
        // liItems변수에 Tag명을 탐색하여 Element 유사배열 할당
        var liItems = document.getElementsByTagName('li');
        liItems[0].style.color = 'blue'; // 첫번째 요소 컬러 변
        liItems[1].style.color = 'blue'; // 두번째 요소 컬러 변경
        liItems[2].style.color = 'blue'; // 번째 요소 컬러 변경
    " />
    <h1>HTML class로 선택하기</h1>
    <ul>
        <li>html : 마크업 언어</li>
        <li>css : html 스타일 언어</li>
        <li>javascript : 동적 언</li>
    </ul>
</body>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/OJpZQBY" %}



