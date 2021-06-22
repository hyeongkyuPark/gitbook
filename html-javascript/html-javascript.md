---
description: HTML에서 JavaScript가 어떤 역할을 하고 어떻게 사용되는지 간략히 정리
---

# HTML과 JavaScript

## 📕 &lt;script&gt; 태그

* JavaScript를 html에서 사용하는 방법으로 script 태그내에서 자바스크립트를 이용해서 웹을 동적으로 활용할 수 있음

```markup
<h1>JavaScript</h1>
<script>
    // html에 쓰는 함수
    document.write(1+1);// 2
</script>
<h1>HTML</h1>
1+1
```

{% embed url="https://codepen.io/hyeongkyupark/pen/JjWvWKj" %}



* HTML에 직접 쓰는것과 다른점은 HTML은 동적이지 않기 때문에 값을 변경할 수 없고, 계산이 따로 불가능한 반면, 자바스크립트는 원한다면 값을 변경 시킬수도 있고, 여러가지 절차에 따라서 값을 가공하여 표현할 수도 있음

## 📕 Event

* html에서는 자바스크립트를 통한 이벤트 속성을 제공하고 있음 \(onclick, onchange 등 [http://html.elex.pe.kr/reference/events](http://html.elex.pe.kr/reference/events) 참고\)

```markup
<!-- alert()는 경고창을 띄우는 자바스크립트 window 객체 메서드 -->
<input type="button" value="hi" onclick="alert('hi')" />
<input type="text" onchange="alert('changed')" />
<input type="text" onkeydown="alert('keydown!')" />
```

{% embed url="https://codepen.io/hyeongkyupark/pen/yLMjMMG" %}

## 📕 콘솔

* 브라우저는 콘솔이라는 기능을 제공하는데, 콘솔은 현제 페이지 내부에서 자바스크립트를 사용해 볼 수 있음 \(F12 또는 마우스 우클릭 - 검사를 통해 개발자 도구 콘솔탭에서 사용 가능\)



